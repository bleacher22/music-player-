<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Music Player UI</title>


  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #eef2f7, #dbeafe);
    }

    
    .container {
      display: flex;
      gap: 25px;
      align-items: center;
    }

    
    .playlist {
      width: 200px;
      padding: 20px;
      background: #ffffff;
      border-radius: 25px;
      box-shadow: 0 15px 30px rgba(0,0,0,0.1);
    }

    .playlist h3 {
      font-size: 16px;
      margin-bottom: 12px;
      color: #1f2933;
    }

    .playlist ul {
      list-style: none;
    }

    .playlist li {
      font-size: 14px;
      padding: 8px;
      margin-bottom: 6px;
      background: #f5f7ff;
      border-radius: 10px;
      color: #374151;
      cursor: pointer;
      transition: 0.3s;
    }

    .playlist li:hover {
      background: #e0e7ff;
    }

    
    .player {
      width: 280px;
      padding: 30px 20px;
      text-align: center;
      background: #ffffff;
      border-radius: 40px 40px 20px 20px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.12);
    }

    .music-icon {
      width: 80px;
      height: 80px;
      margin: auto;
      border-radius: 50%;
      background: #f0f4ff;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 32px;
      color: #4f46e5;
      animation: float 2.5s ease-in-out infinite;
    }

    h2 {
      margin-top: 15px;
      font-size: 18px;
      color: #1f2933;
    }

    p {
      font-size: 13px;
      color: #6b7280;
      margin-bottom: 18px;
    }

    
    .controls {
      display: flex;
      justify-content: space-around;
      margin-bottom: 15px;
    }

    button {
      width: 45px;
      height: 45px;
      border-radius: 50%;
      border: none;
      background: #eef2ff;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #c7d2fe;
    }

    .play {
      background: #4f46e5;
      color: white;
    }

    .play:hover {
      background: #4338ca;
    }

    
    .timeline {
      width: 100%;
      height: 6px;
      background: #e5e7eb;
      border-radius: 10px;
      overflow: hidden;
      margin-bottom: 6px;
    }

    .progress {
      width: 40%; 
      height: 100%;
      background: #4f46e5;
      border-radius: 10px;
    }

    
    .time {
      display: flex;
      justify-content: space-between;
      font-size: 12px;
      color: #6b7280;
    }

    
    @keyframes float {
      0%,100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }
  </style>
  

</head>
<body>

<div class="container">

  
  <div class="playlist">
    <h3>My Playlist</h3>
    <ul>
       <li>🎵 Manasilayo</li>
      <li>🎵 Kadhal-Asai </li>
      <li>🎵 Kannama</li>
      <li>🎵 Enna-villai</li>
      <li>🎵 Jimmiki Ponnu</li>
    </ul>
  </div>

  
  <div class="player">
    <div class="music-icon">🎶</div>

    <h2>Now Playing</h2>
    <p>En-Uyire</p>

    <div class="controls">
      <button>⏮</button>
      <button class="play">▶</button>
      <button>⏭</button>
    </div>

    <div class="timeline">
      <div class="progress"></div>
    </div>

    <div class="time">
      <span>1:50</span>
      <span>3:45</span>
    </div>
  </div>

</div>

</body>
</html>
