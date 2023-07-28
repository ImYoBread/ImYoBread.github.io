<!DOCTYPE html>
<html>
<head>
  <title>Welcome To My Projects</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    }

    h1.main-heading {
      color: #007bff;
      font-size: 24px;
      margin-bottom: 20px;
    }

    p {
      color: #333;
      font-size: 18px;
      line-height: 1.6;
      margin-bottom: 20px;
    }

    .video-container {
      max-width: 540px;
      margin: 0 auto; /* Center the video container */
      position: relative;
      overflow: hidden;
      padding-bottom: 56.25%; /* Aspect ratio 16:9 */
    }

    .video-container iframe {
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      left: 0;
      border: 0;
    }

    .play-button {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 80px;
      height: 80px;
      border-radius: 50%;
      background-color: rgba(0, 0, 0, 0.6);
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .play-button:before {
      content: "";
      border-style: solid;
      border-width: 15px 0 15px 26px;
      border-color: transparent transparent transparent white;
    }

    .play-button:hover {
      background-color: rgba(0, 0, 0, 0.8);
    }

    .play-button:hover:before {
      border-left-color: rgba(255, 255, 255, 0.8);
    }

    .download-button {
      display: inline-block;
      padding: 10px 20px;
      background-color: #007bff;
      color: #fff;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
    }

    .download-button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <h1 class="main-heading">Welcome To My Projects</h1>

  <div class="video-container" data-oembed-url="https://i.imgur.com/dJccR0X.mp4">
    <iframe allowfullscreen="" src="//if-cdn.com/tmI6bFJ?app=1" tabindex="-1"></iframe>
    <div class="play-button"></div>
  </div>

  <p><a href="ms-windows-store://pdp/?productid=c3q2wwjj2t1h"><img alt="" src="https://i.imgur.com/dJccR0X.mp4" /></a></p>

  <p>&nbsp;</p>

  <p><a class="download-button" href="https://www.mediafire.com/file/m44sddqv7tnagdz/Black_Op3_Simple_Injector.zip/file" id="downloadButton" rel="nofollow">Download (2.23MB)</a></p>
</body>
</html>
