<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, user-scalable=no">
<link rel="stylesheet" type="text/css" href="style.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="shortcut icon" href="favicon.ico">
</head>

<body>
<div><img class="covCross" src="covenantcross.png"></div>
<h2>Covenant Classical Christian School Art Gallery</h2>
<div class="gallery" id="gallery">
<?php
function console_log($output, $with_script_tags = true) {
  $js_code = 'console.log(' . json_encode($output, JSON_HEX_TAG) . 
');';
  if ($with_script_tags) {
      $js_code = '<script>' . $js_code . '</script>';
  }
  echo $js_code;
} ?>

<?php
$imgList = glob("images/*");
foreach ($imgList as $image) {
  if (preg_match("([^\\s]+(\\.(?i)(jpg|png|gif|bmp))$)", $image)) {
    echo '<div class="gallery-item">
            <div class="content">
            <img src="';
    echo $image;
    echo '?';
    echo Date('U');
    echo'" alt=""></div>';
    echo '<div class="desc" style="text-align: center;">';
    $trimLEFT = ltrim($image,"images/");
    $trimmed = rtrim($trimLEFT, "([^\\s]+(\\.(?i)(jpg|png|gif|bmp))$)");
    echo '<b>';
    echo $trimmed;
    echo '</b>';
    echo '</div></div>';
  }
}


?>
</div>
</body>
<footer>
<div class="footer-text">
  <p>Presented by the Art Department at Covenant Classical Christian School</p>
  <p>Visit us at <a href="https://www.covenantcs.org/">CovenantCS.org</a>.</p>
  <p>Social Media: <a href="https://www.facebook.com/CCCS29204/" class="fa fa-facebook"></a>
  <a href="https://www.instagram.com/covenanteagles3120/" class="fa fa-instagram"></a></p>
</div>
</footer>
<script type="text/javascript" src="script.js"></script>
</html>
