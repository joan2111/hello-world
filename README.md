<!doctype html>

<head>
<title>Homepage</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
<link rel="stylesheet" href="webseite.css" style="css">
<script type="text/javascript" src="javascript.js"></script>
<link rel="stylesheet" href="https://netdna.bootstrapcdn.com/font-awesome/4.0.3/css/font-awesome.min.css">
<link href="https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>

<script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>





</head>

<body>

  <?php
  if(isset($_POST["submit"])){
        mail("tutorialworktv@gmail.com", "Kontaktformular", 'Name: '.$_POST["name"].' Email: '.$_POST["email"].' Betreff: '.$_POST["subject"].' Telefon: '.$_POST["telefon"].' Nachricht: '.$_POST["message"]);
        ?>
        <h1 style="color: green;">Das Kontaktformular wurde abgesendet!</h1>
        <?php
      }
       ?>


<!-- Header --->
<section class="sec1">
<header>
<nav id="pointermenu2">
  <ul>
  <li><a href="index.html">Home</a></li>
  <li><a href="#images">Referenzen</a></li>
  <li><a href="#form">Kontakt</a></li>
</ul>
</nav>
</header>
<!-- Header --->

<div class="fade-in">
  <h1 id="text">Willkommen!</h1>
</div>


<!--- acordion ----->
<div id="main">
<div class="fade-in" style="margin-top:100px;">
<input type="radio" id="animal" name="wiki" value="Animal" checked>
<input type="radio" id="plant" name="wiki" value="Plant">
<input type="radio" id="space" name="wiki" value="Space">
<input type="radio" id="river" name="wiki" value="River">

<ul class="accordion">
  <li data-radio="animal">
    <label for="animal" class="accordion-title">
      <span>01</span>
      <span class="accordion-heading">Über mich</span>
    </label>
    <div class="accordion-content">Mein Name ist Joan Gulich. Ich bin ein leidenschaftlicher Programmierer und heiße Sie herzlich willkommen auf meiner Webseite. Hier erfahren sie mehr über mich und meiner Arbeit und Erfahrungen die ich auf dem weg zu einem Webdeveloper machen konnte.  </div>
  </li>
  <li data-radio="plant">
    <label for="plant" class="accordion-title">
      <span>02</span>
      <span class="accordion-heading">Programmiersprachen</span>
    </label>
    <div class="accordion-content">Programmiersprachen:<br>HTML 5<br>CSS<br>Java script<br>JQuery<br>Bootsrap<br>PHP<br></div>
  </li>
  <li data-radio="space">
    <label for="space" class="accordion-title">
      <span>03</span>
      <span class="accordion-heading">Erfahrungen</span>
    </label>
    <div class="accordion-content">Zertifikate im Berreich Webdesign über die Seite Udemy.com und Programmierer Zerftifikate über die App Mimo.Zudem habe ich durch viel selbst rechachieren selbst angeeignet und erfolgreich umgesetzt.</div>
  </li>
  <li data-radio="river">
    <label for="river" class="accordion-title">
      <span>04</span>
      <span class="accordion-heading">Programm-kenntnisse</span>
    </label>
    <div class="accordion-content">Programme:<br>Adobe Photoshop<br>Adobe XD<br>Adobe Illustrator<br>Adobe InDesign<br>Adobe Dreamweaver<br>und vieles mehr...</div>
  </li>
</ul>
</div>
</div>

</section>
<!--- acordion ----->

<!--- main ----->
<div id="middle">



<div class="wrapper">
    <div class="counter col_fourth">
      <i class="fa fa-code fa-2x"></i>
      <h2 class="timer count-title count-number" data-to="300" data-speed="5000"></h2>
       <p class="count-text ">Programmierungen</p>
    </div>

    <div class="counter col_fourth">
      <i class="fa fa-coffee fa-2x"></i>
      <h2 class="timer count-title count-number" data-to="1700" data-speed="5000"></h2>
      <p class="count-text ">Kaffee Tassen</p>
    </div>

    <div class="counter col_fourth">
      <i class="fa fa-lightbulb-o fa-2x"></i>
      <h2 class="timer count-title count-number" data-to="11900" data-speed="5000"></h2>
      <p class="count-text ">Projekte</p>
    </div>

    <div class="counter col_fourth end">
      <i class="fa fa-bug fa-2x"></i>
      <h2 class="timer count-title count-number" data-to="157" data-speed="5000"></h2>
      <p class="count-text ">Kunden</p>
    </div>
</div>

</div>
<!--- main ----->

<!--- Referenzen ----->
<section class="sec2">

  <div id="images">
    <img id="image1" src="Landingpage.jpg" />
    <img id="image2" src="Bootsrap-website.jpg" />
    <img id="image3" src="Website-layout.jpg" />
    <img id="image4" src="webseite layout.jpg" style=""  />
  </div>
  <div id="slider">
    <a href="#image1">1</a>
    <a href="#image2">2</a>
    <a href="#image3">3</a>
    <a href="#image4">4</a>
  </div>





</section>
<!--- Referenzen ----->





<!--- Kontakt ----->
<div id="last">
<h2 style="display:inline-block;"> Kontakt</h2>
</div>

<section class="sec3">

<div id="form">
  <div class="contain">

       <div class="wrapp animated bounceInLeft">
           <div class="company-info">
               <h3>Kontakt</h3>
               <ul>
                   <li class="li_form"><i class="fa fa-road"></i> 47807, Krefeld</li>
                   <li class="li_form"><i class="fa fa-phone"></i> &nbsp;015736482483</li>
                   <li class="li_form"><i class="fa fa-envelope"></i> joangulich@web.de</li>
               </ul>
           </div>

           <div class="contact">
               <h3>Kontaktiere mich</h3>
               <form action="index.php" method="post">
                   <p>
                       <label>Name</label>
                       <input type="text" name="name">
                   </p>
                   <p>
                       <label>Betreff</label>
                       <input type="text" name="subject">
                   </p>
                   <p>
                       <label>Email Addresse</label>
                       <input type="email" name="email">
                   </p>
                   <p>
                       <label>Telefon</label>
                       <input type="numbers" name="telefon" >
                   </p>
                   <p class="full">
                       <label>Nachricht</label>
                       <textarea name="message" rows="5" ></textarea>
                   </p>
                   <p class="full">
                       <button  name="submit" type="submit">Senden</button>
                   </p>
               </form>
           </div>
       </div>
   </div>
</div>
</section>

<!--- kontakt ----->

<!--- footer ----->
<div id="footer">



<div class="content1">

<footer>
  <div class="footer footer__wrapper">
    <div class="footer__left">
      <ul class="footer__social-media">

        <li class="li_footer">
          <a href="https://www.facebook.com/"><i class="fa fa-facebook fa-lg sm-item" aria-hidden="true"></i></a>
        </li>

      <li class="li_footer">
          <a href="https://twitter.com"><i class="fa fa-twitter fa-lg sm-item" aria-hidden="true"></i></a>
        </li>

        <li class="li_footer">
          <a href="https://linkedin.com"><i class="fa fa-linkedin-square fa-lg sm-item" aria-hidden="true"></i></a>
        </li>

      <li class="li_footer">
          <a href="https://youtube.com"><i class="fa fa-youtube fa-lg sm-item" aria-hidden="true"></i></a>
        </li>
      </ul>
      <p class="footer__text">&#169;Joan Gulich | <a href="#">Terms &amp; Impressum</a> | <a href="">Datenschutz</a></p>
    </div>
    <div class="footer__right">
      <a href="#"><img src="http://via.placeholder.com/150x50" class="footer__logo"></a>
    </div>
  </div>
</footer>
  </div>
</div>
<!--- footer ----->




<script type="text/javascript" src="javascript.js"></script>


</body>




</html>
