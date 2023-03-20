<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            height: 1000px;
        }
        button{
            background-color: red;
            border-radius: 20px;
            position:fixed;
            bottom:10px;
            right:10px;
            display:none;
        }
    </style>
</head>
<body>
    <button>Go Up</button>

    <script>
        var btn=document.querySelector("button");
        window.onscroll=function(){
            if (window.scrollY>200){
                btn.style.display="block";
            }
            else{
                btn.style.display="none";
            }
        }
        btn.onclick=function(){
            window.scroll(0,0)
        }

    </script>
</body>
</html>
