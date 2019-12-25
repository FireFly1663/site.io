# site.io
Our project

<!DOCTYPE html>

<html>
	<head>
		<meta charset="utf-8">
		<title>Анкета для вступу</title>
		<link rel="stylesheet" type="text/css" href="2cs.css">
		

	</head>
	
	<body background="as.jpg">
	
		<header>
			<p id="header1"> Фізико-Технічний Інститут</p>
		</header>

		<div id="a1">
		
			<div id="bord">
				Ваше фото
			</div>



			<form id="regform" method="POST" action="valid.php">
       		 <h1 class="whcol">Registration</h1>
    </h1>
                    <hr>
                    <p align="left"><label for="name"><b class="regist">Имя
   </b>

                        </label>
                        <input type="text" placeholder="Enter Your Name" name="name" id="name" >

                    </p>
                       <span class="error"></span>     
                    <p align="left">
                        <label for="surname"><b class="regist">Фамилия
   </b>
                        </label>
                        <input type="text" placeholder="Enter Your Surname" name="surname" id="surname" >
                        <span class="error"></span>
                    </p>
        

                    <p align="left">
                        <label for="email"><b class="regist">Email
   </b>
                        </label>

                        <input type="email" placeholder="Enter Email" name="email" id="email" >
                        <span class="error"></span>
                    </p>

                    <p align="left">
                        <label for="psw"><b class="regist">Пароль
    </b>
                        </label>

                        <input type="password" placeholder="Enter Password" name="psw" id="password" >
                        <span></span>
                    </p>
 
                    <p align="left">
                        <label for="psw-repeat"><b class="regist">Повтор</b>
                        </label>

                        <input type="password" placeholder="Repeat Password" name="psw-repeat" id="confirm_password" >
                        <span></span>
                    </p>

                    <hr>
                    <button type="submit" class="button" name="submit">Регистрация
                    </button>


           </div></br></br>

          

			</form>
		</div>
	</body>

	<script src="jquery-3.4.1.min.js"></script>
	<script src="jquery_validation.js"></script>
	<script src="script.js"></script>
	<script>
	 $.validator.setDefaults({ ignore: "#email" });
	  $('#regform').validate({
	    rules : {
	                password : {
	                    minlength : 8
	                },
	                confirm_password : {
	                    minlength : 8,
	                    equalTo : "#password"
	                },
	                ignore: "*"
	                
	            }
	});
	</script>

</html>
