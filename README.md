# ramy-helmy.github.io
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dr.Ramy-Helmy</title>
  <style>
    html {
      scroll-behavior: smooth;
    }

    * {
      padding: 0;
      margin: 0;
      box-sizing: border-box;
      -webkit-box-sizing: border-box;
      -moz-box-sizing: border-box;
      -o-box-sizing: border-box;
    }

    div.container {
      max-width: 100vw;
      max-height: 6332px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    img {
      max-width: 100%;
    }

    div.container a {
      width: 80px;
      height: 80px;
      position: fixed;
      bottom: 50px;
      right: 50px;
      border-radius: 50%;
      transform: scale(1);
      transition: 0.2s;
      animation: ease;
      background-color: #d03f3e;
      z-index: 2;
    }

    @media (max-device-width: 768px) {
      div.container a {
        transform: scale(0.5);
        bottom: 20px;
        right: 20px;
      }
    }

    div.fixedBtn {
      width: 40px;
      height: 40px;
      transform-origin: center;
      transform: translate(50%, 70%) rotate(-45deg);
      animation: ease;
      transition: all 0.1s;
      border: 10px solid white;
      border-bottom: none;
      border-left: none;
    }

    div.fixedBtn::before {
      content: "";
      position: absolute;
      width: 10px;
      height: 40px;
      transform-origin: bottom;
      transform: translate(25%, -45%) rotate(45deg) scaleY(0);
      background-color: white;
      animation: ease;
      transition: all 0.05s;
    }

    div.container a:hover {
      background-color: #000;
    }

    div.container a:hover div.fixedBtn {
      transform: translate(50%, 50%) rotate(-45deg);
    }

    div.container a:hover div.fixedBtn::before {
      transform: translate(25%, -45%) rotate(45deg) scaleY(1);
    }
  </style>
</head>

<body>
  <div class="container" id="top">
    <img src="Landing-Page.png" alt="Landing-Page">
    <a href="#top" title="Go Top">
      <div class="fixedBtn"></div>
    </a>
  </div>
</body>

</html>
