# build-for-bharath
hackthon
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Shopping Assistant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: black;
        }
        
        .label{
            width: 75%;
            height: 20%

        
        }
        .head{
            color: red;
        }
        .butt{
            width: 130px;
            height: 50px;
            background-color: none;
            border: solid black;
            cursor: pointer;
        }
        .butt:hover{
            background-color: rgb(230, 91, 91);
            color: white;
            transition: .5s;
        }
        #occasionInput{
            width: 300px;
            height: 40px;
        }
        p{
            color: red;
        }
       

    </style>
</head>
<body>
    <div class="head">
    <h1 >Cybertron7-chatbot</h1>
    <h2 >Welcome to our online shopping assistant!</h2>
<div>
    <img src="https://th.bing.com/th/id/OIP.qYeI5HSSlpOElryURb5VlQHaE6?pid=ImgDet&w=197&h=130.8203125&c=7&dpr=1.3" alt="" > <h2> Marrige</h2>
    <img src="https://th.bing.com/th/id/OIP.5TWT9LRwY37BoJ_3-sfTdwHaEK?rs=1&pid=ImgDetMain" alt=""> <h2>gift</h2>
    <img src="https://th.bing.com/th/id/OIP.PCwuRdhAYoq0NzRfU2WgSgHaFO?pid=ImgDet&w=197&h=138.92604166666666&c=7&dpr=1.3" alt=""> <h2>diwali</h2>
    <img src="https://www.edudwar.com/wp-content/uploads/2021/02/Sankranti.jpeg" alt=""> <h2>sankranti</h2>
   

</div>
</div>
    <div class="label">
   <h2> <label for="occasionInput" style="color: red;">Enter the occasion:</label></h2>
    <input type="text" id="occasionInput">
    <button onclick="openWebsite()" class="butt">Go</button>
    </div>
    

    <p id="resultMessage"></p>

    <script>
        function openWebsite() {
            var userInput = document.getElementById('occasionInput').value.toLowerCase();
            var occasionLinks = {
                'marrige': 'https://www.flipkart.com/search?q=marrige&otracker=search&otracker1=search&marketplace=FLIPKART&as-show=on&as=off',
                'gift': 'https://www.bing.com/search?q=gifts&qs=n&form=QBRE&sp=-1&ghc=1&lq=0&pq=gifts&sc=11-5&sk=&cvid=865B69C396A14579B79035916578979E&ghsh=0&ghacc=0&ghpl=',
                'diwali':'https://www.bing.com/search?q=diwali+&qs=n&form=QBRE&sp=-1&ghc=1&lq=0&pq=diwali+&sc=11-7&sk=&cvid=EB518AED0BA745559A68C14D668FA868&ghsh=0&ghacc=0&ghpl=',
                'sankranti':'https://www.bing.com/search?q=sankranti+shopping&qs=n&form=QBRE&sp=-1&ghc=1&lq=0&pq=sankranti+shoppin&sc=9-17&sk=&cvid=DCAA09FCFBB64092B5CBABDC91C63EDB&ghsh=0&ghacc=0&ghpl='
            };

            if (occasionLinks[userInput]) {
                window.open(occasionLinks[userInput], '_blank');
                document.getElementById('resultMessage').innerText = '';
            } else {
                document.getElementById('resultMessage').innerText = 'No specific action defined for \'' + userInput + '\'. Provide a valid keyword.';
            }
        }
    </script>
</body>
</html>
