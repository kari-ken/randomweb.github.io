
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>randomweb</title>
  <style>
    body, html {
      margin: 0; padding: 0; height: 100%;
      background-color: #000;
      color: #f00;
      font-family: 'Arial Black', Arial, sans-serif;
      overflow-y: scroll;
    }

   .container {
      max-width: 900px;
      margin: 20px auto 70px;
      background: #111;
      border: 3px solid #f00;
      border-radius: 10px;
      display: flex;
      gap: 20px;
      padding: 15px;
    }

  .left-column {
      flex: 1 1 250px;
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

  .right-column {
      flex: 2 1 600px;
      display: flex;
      flex-direction: column;
      gap: 20px;
    }

  .profile-box, .contact-box, .interests-box, .info-box, .box-container {
      background: #220000;
      border: 2px solid #f00;
      padding: 15px;
      border-radius: 8px;
      font-size: 14px;
      color: #f00;
    }

   .section-title, .box-header {
      background: #f00;
      color: #000;
      font-weight: bold;
      padding: 5px 10px;
      margin-bottom: 10px;
      border-radius: 4px;
      text-align: center;
    }

  .profile-pic {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 3px solid #f00;
      margin-bottom: 10px;
      object-fit: cover;
    }
  
  .profile-name {
      font-size: 28px;
      font-weight: bold;
      margin-bottom: 5px;
      text-align: center;
    }

   .profile-info {
      font-size: 14px;
      line-height: 1.3;
      text-align: center;
    }

   ul {
      padding-left: 20px;
      margin: 0;
    }

   a {
      color: #f00;
      text-decoration: underline;
    }

  .image-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
      gap: 8px;
    }

   .image-box {
      background: black;
      border: 1px dotted #f00;
      height: 70px;
      border-radius: 6px;
      cursor: pointer;
    }

   .mp3-box {
      background: #220000;
      border: 2px solid #f00;
      border-radius: 8px;
      padding: 5px 10px;
      max-width: 300px;
      margin: 10px auto;
      display: flex;
      align-items: center;
      gap: 10px;
      justify-content: center;
      box-shadow: 0 0 8px #f00;
    }

   .mp3-box label {
      color: #f00;
      font-weight: bold;
      font-size: 12px;
      user-select: none;
    }

   .mp3-box audio {
      width: 180px;
      outline: none;
      filter: drop-shadow(0 0 2px #f00);
      border-radius: 6px;
    }

  .profile-pic.spin {
      animation: spin 20s linear infinite;
    }

  @keyframes spin {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

   #vinyl-gallery-container {
      display: flex;
      gap: 20px;
      flex-wrap: nowrap;
      justify-content: space-between;
    }

   #vinyl-gallery-1, #vinyl-gallery-2 {
      background: #220000;
      border: 2px solid #f00;
      border-radius: 8px;
      width: 48%;
      padding: 10px;
      display: flex;
      gap: 12px;
      overflow-x: auto;
      scroll-behavior: smooth;
    }

  .vinyl {
      perspective: 500px;
      width: 22px;
      transition: width 0.5s;
      flex-shrink: 0;
      cursor: pointer;
      border-radius: 4px;
    }

   .vinyl:hover {
      width: 150px;
    }

  .vinyl img {
      width: 150px;
      height: 150px;
      border-radius: 4px;
      border: 2px solid rgba(255, 0, 0, 0.6);
      object-fit: cover;
      transition: transform 0.5s, width 0.5s, height 0.5s, margin-top 0.5s;
      transform-style: preserve-3d;
      transform: rotateX(0deg) rotateY(25deg);
    }

  .vinyl:hover img {
      transform: rotateX(0deg) rotateY(10deg);
      width: 158px;
      height: 158px;
      margin-top: -2px;
    }
  </style>
</head>
<body>

<div class="container">
  <!-- Left column -->
  <div class="left-column">
    <div class="profile-box">
      <img src="https://i.imgur.com/DfQX9zN.png" alt="Profile Pic" class="profile-pic spin" />
      <div class="profile-name">stuff</div>
      <div class="profile-info">
        stuff<br />
          <br />
          stuff<br /><br />
              stuff <br />
      
  </div>
    </div>

   <div class="contact-box">
      <div class="section-title"> stuff</div>
      <ul>
        <li> s s</li>
        <li>stuff</li>
        <li>stuf</li>
        <li>stuff</li>
        <li>stuff</li>
        <li>stuff</li>
        <li>stuff</li>
      </ul>
      <small> stuff</small>
    </div>

  <div class="interests-box">
      <div class="section-title">stuff</div>
      <p><strong>General</strong><br />
        stuff
      </p>
      <p>stuff<br />
        <a href="#" style="color:#f00;">HOMESTUCK</a>
      </p>
      <img src="https://i.imgur.com/YQCyCPH.png" alt="Interest Image" style="width:100%; border-radius: 6px;"/>
    </div>
  </div>

  <!-- Right column -->
  <div class="right-column">
    <!-- Vinyl Galleries -->
    <div id="vinyl-gallery-container">
      <div id="vinyl-gallery-1">
        <a href="https://example.com/artist1-album1" target="_blank" class="vinyl"><img src="https://i.imgur.com/fQk3Hln.png" alt="Artist 1 - Album 1" /></a>
        <a href="https://example.com/artist2-album2" target="_blank" class="vinyl"><img src="https://i.imgur.com/K9y2p38.png" alt="Artist 2 - Album 2" /></a>
        <a href="https://example.com/artist3-album3" target="_blank" class="vinyl"><img src="https://i.imgur.com/v8hJUoR.png" alt="Artist 3 - Album 3" /></a>
        <a href="https://example.com/artist4-album4" target="_blank" class="vinyl"><img src="https://i.imgur.com/EdN2pWZ.png" alt="Artist 4 - Album 4" /></a>
        <a href="https://example.com/artist5-album5" target="_blank" class="vinyl"><img src="https://i.imgur.com/1Y5FJbW.png" alt="Artist 5 - Album 5" /></a>
        <a href="https://example.com/artist6-album6" target="_blank" class="vinyl"><img src="https://i.imgur.com/5HKfwU9.png" alt="Artist 6 - Album 6" /></a>
        <a href="https://example.com/artist7-album7" target="_blank" class="vinyl"><img src="https://i.imgur.com/qB5nY6S.png" alt="Artist 7 - Album 7" /></a>
      </div>

   <div id="vinyl-gallery-2">
        <a href="https://example.com/artist8-album8" target="_blank" class="vinyl"><img src="https://i.imgur.com/g7KuNaR.png" alt="Artist 8 - Album 8" /></a>
        <a href="https://example.com/artist9-album9" target="_blank" class="vinyl"><img src="https://i.imgur.com/pX1Zct2.png" alt="Artist 9 - Album 9" /></a>
        <a href="https://example.com/artist10-album10" target="_blank" class="vinyl"><img src="https://i.imgur.com/gwgHQUV.png" alt="Artist 10 - Album 10" /></a>
        <a href="https://example.com/artist11-album11" target="_blank" class="vinyl"><img src="https://i.imgur.com/3cXhLQz.png" alt="Artist 11 - Album 11" /></a>
        <a href="https://example.com/artist12-album12" target="_blank" class="vinyl"><img src="https://i.imgur.com/PNxuNRa.png" alt="Artist 12 - Album 12" /></a>
        <a href="https://example.com/artist13-album13" target="_blank" class="vinyl"><img src="https://i.imgur.com/2ntnDwl.png" alt="Artist 13 - Album 13" /></a>
        <a href="https://example.com/artist14-album14" target="_blank" class="vinyl"><img src="https://i.imgur.com/MafT79h.png" alt="Artist 14 - Album 14" /></a>
      </div>
    </div>
   <!-- New info boxes -->
    <div class="info-box">
      <div class="section-title">v games</div>
      <p>stuff</p>
    </div>

  <div class="info-box">
      <div class="section-title">Mood</div>
      <p>stuff</p>
    </div>

   <div class="info-box">
      <div class="section-title">Favorites</div>
      <ul>
        <li>stuff</li>
        <li>stuff</li>
        <li>stuff</li>
      </ul>
    </div>

    <!-- Added sections you requested -->
  <div class="info-box">
      <div class="section-title">stuff</div>
      <p>stuff</p>
    </div>

  <div class="info-box">
      <div class="stuff">Movies</div>
      <p>stuff</p>
    </div>

  <div class="info-box">
      <div class="section-title">Horror</div>
      <p>stuf.</p>
    </div>

   <div class="info-box">
      <div class="section-title">Video Games</div>
      <p>stuff</p>
    </div>

   <!-- Photos box -->
<div class="box-container">
      <div class="box-header">Photos</div>
      <div class="image-grid">
        <!-- 80 empty boxes for images -->
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
        <div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div><div class="image-box"></div>
      </div>
    </div>
  </div>
</div>

<div class="mp3-box">
  <label for="player">PLAY MUSIC:</label>
  <audio controls id="player">
    <source src="https://files.freemusicarchive.org/storage-freemusicarchive-org/music/ccCommunity/iiammike/Studio_iiammike/iiammike_-_Starfox.mp3" type="audio/mpeg" />
    Your browser does not support the audio element.
  </audio>
</div>

</body>
</html>
