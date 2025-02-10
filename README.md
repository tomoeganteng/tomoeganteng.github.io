<!DOCTYPE html>
<html lang="en">
    <head>
        <link rel="stylesheet" href="./styles.css">
        
    </head> 
    <body>
        <div class="container">
            <div >
                <h1 class = "header_text">Do you wanna be my valentine?</h1>
                <h1 class = "header_text">I don't accept no for an answer 🙂</h1>
            </div>
            <div class="gif_container">
                <img src="https://i.pinimg.com/originals/68/67/a6/6867a6471c4968d4d9998771c76ca522.gif">
            </div>
            <div class = "buttons">
                <button class="btn" id = "yesButton" onclick="nextPage()">Yes</button>
                <button class="btn" id="noButton" onmouseover="moveButton()" onclick="moveButton()">No</button>
                <script>
                    function nextPage() {
                        window.location.href = "yes.html";
                    }
                    
                    function moveButton() {
                        var x = Math.random() * (window.innerWidth - document.getElementById('noButton').offsetWidth) - 85;
                        var y = Math.random() * (window.innerHeight - document.getElementById('noButton').offsetHeight) - 48;
                        document.getElementById('noButton').style.left = `${x}px`;
                        document.getElementById('noButton').style.top = `${y}px`;
                    }
                </script> 
            </div>
        </div>
       
    </body> 
</html>
