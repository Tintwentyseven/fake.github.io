<!DOCTYPE html>
<!DOCTYPE html>
<br lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="project3.css"/>
    <title>Registration form</title>
    <script src="https://code.jquery.com/jquery-3.6.1.min.js" integrity="sha256-o88AwQnZB+VDvE9tvIXrMQaPlFFSUTR+nldQm1LuPXQ=" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@10"></script>
    <!-- <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script> -->
</head>
<body >
<div class="container">
    <img src="https://i.pinimg.com/736x/61/8a/74/618a7401f69608d55b14c46e15efbc4b.jpg" width="100px" height="100px">

        <h1>Contract us</h1>
        <form>
            
            <div class="Send1">
                <input type="text" id="Uppername" class="field1" placeholder="Your Name" onblur="Upper()" style="caret-shape:underscore;caret-color: blue;">
                <input type="submit" value="Send">
            </div>
            <div class="Send2">
                <input type="password" class="field1" placeholder="Your password">
                <input type="submit" value="Send">
            </div>
            <p id="I"><span><input type="checkbox"></span>I agree the terms of services</p>
            <button type="button" id="signup_bn" onclick="getDate()">Sign up</button>
            <br><br>
            <hr style="border:  solid red;">
            <p class="OR">Or</p>
            <br>
            <button type="buton" id="signup_bn1">Login with twitter</button>
            <p>Do you have an accounts? <a href="#">Sign in</a></p>
            
         
        
    </div>
</div>

      <style>
        p::selection{
            color: aqua;
            background: orangered;
        }
        #I{
            user-select: none;
        }
      </style>      
      <script>
        // $(document).ready(function(){
        //     $('#signup_bn').click(function(){
        //         $('#I').append('Cho');
        //     })
        // })
       
        // function getDate(){
        //     alert(new Date($.now()));
        // }
   
            $('signup_bn').click(function(){

                $('#signup_bn1').attr("disabled", true);
            });
     
   

        $(document).ready(function(){
            $('#signup_bn1').click(function(){
                if($("input[type=checkbox]").filter(":checked").length < 1){
                    alert("Please enter");
                }
            })
        })
        $(document).ready(function(){
            $(document).bind("contextmenu",function(event){
                alert("Right click is disabled");
                return false;
            });
        })
function Upper(){
   var x = document.getElementById("#Uppername");
   x.value = x.value.toUpperCase();
}


       
            
      </script>
        


</body>
</html>

