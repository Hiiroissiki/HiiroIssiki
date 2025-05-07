<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Film</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      background: #0a0a0a;
      color: #d9d9d9;
      font-family: 'Cormorant Garamond', serif;
      overflow-x: hidden;
    }
    .video-container {
      position: relative;
      min-height: 100vh;
      padding: 40px;
      background: #0a0a0a;
      transition: background 0.3s;
    }
    .video {
      position: absolute;
      z-index: 1;
      opacity: 1;
    }
    .video iframe {
      border: none;
      box-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
      width: 100%;
      height: 100%;
    }
    .poem-en {
      position: absolute;
      z-index: 2;
      color: #666;
      font-size: 1.2em;
      opacity: 1;
      pointer-events: none;
    }
    .matrix-text {
      position: absolute;
      z-index: 0;
      color: #666;
      font-size: 0.9em;
      white-space: nowrap;
      text-shadow: 0 0 5px rgba(255, 255, 255, 0.7);
      pointer-events: none;
      transition: opacity 0.5s;
    }
    .releases, .sns-contact {
      position: relative;
      z-index: 2;
      max-width: 1200px;
      margin: 0 auto;
      padding: 40px 20px;
      text-align: center;
      background: #0a0a0a;
      transition: background 0.3s;
    }
    .releases h2, .sns-contact h2 {
      font-size: 2em;
      margin-bottom: 20px;
      opacity: 0;
      animation: fadeIn 2s forwards;
    }
    .album-grid {
      display: flex;
      flex-direction: column;
      gap: 20px;
      margin-bottom: 20px;
    }
    .album-item {
      text-align: center;
    }
    .album-item span {
      font-size: 1.5em;
      color: #999;
      display: block;
      margin-bottom: 5px;
    }
    .album-links a {
      color: #999;
      font-size: 0.9em;
      margin: 0 10px;
      text-decoration: none;
      transition: color 0.3s;
    }
    .album-links a:hover {
      color: #fff;
    }
    .sns-contact {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .sns-contact a {
      color: #999;
      font-size: 2em;
      margin: 10px;
      transition: color 0.3s;
    }
    .sns-contact a:hover {
      color: #fff;
    }
    .contact p {
      margin-top: 20px;
      font-size: 1.2em;
      color: #999;
    }
    @keyframes fadeIn {
      to { opacity: 1; }
    }
    @media (max-width: 768px) {
      .video-container {
        display: flex;
        flex-direction: column;
        gap: 20px;
        padding: 20px;
      }
      .video {
        position: static !important;
        top: auto !important;
        left: auto !important;
        width: 100% !important;
        height: 200px !important;
      }
      .video iframe {
        width: 100% !important;
        height: 100% !important;
      }
      .poem-en {
        font-size: 1em;
        top: 10px !important;
        left: 10px !important;
      }
      .matrix-text {
        font-size: 0.7em;
      }
      .releases h2, .sns-contact h2 {
        font-size: 1.8em;
      }
      .album-item span {
        font-size: 1.3em;
      }
      .sns-contact a {
        font-size: 1.5em;
      }
      .contact p {
        font-size: 1em;
      }
    }
  </style>
</head>
<body>
  <div class="video-container">
    <!-- 動画：YouTube 9個＋Sounding Garden＋Vimeo、PC：固定配置、スマホ：縦並び -->
    <div class="video" style="top: 10%; left: 5%; width: 300px; height: 168.75px;">
      <iframe src="https://www.youtube.com/embed/qYGZoM73NZ8" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 15%; left: 50%; width: 350px; height: 196.875px;">
      <iframe src="https://www.youtube.com/embed/aDCCKP64Qpk" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 40%; left: 20%; width: 280px; height: 157.5px;">
      <iframe src="https://www.youtube.com/embed/AyYrFHW7pqs" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 60%; left: 70%; width: 320px; height: 180px;">
      <iframe src="https://www.youtube.com/embed/9Pkux-P1UcE" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 70%; left: 10%; width: 200px; height: 112.5px;">
      <iframe src="https://www.youtube.com/embed/Xi-gQog4VpY" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 20%; left: 35%; width: 200px; height: 112.5px;">
      <iframe src="https://www.youtube.com/embed/xasHkPjtO_g" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 50%; left: 45%; width: 200px; height: 112.5px;">
      <iframe src="https://www.youtube.com/embed/IgQtqrPU1Jk" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 80%; left: 25%; width: 200px; height: 112.5px;">
      <iframe src="https://www.youtube.com/embed/Kxy2gIV8zB0" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 30%; left: 80%; width: 200px; height: 112.5px;">
      <iframe src="https://www.youtube.com/embed/a5DZQnQ6U84" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 50%; left: 5%; width: 300px; height: 168.75px;">
      <iframe src="https://soundinggarden.org/" allowfullscreen></iframe>
    </div>
    <div class="video" style="top: 25%; left: 65%; width: 280px; height: 157.5px;">
      <iframe src="https://player.vimeo.com/video/911984780" allowfullscreen></iframe>
    </div>
    <!-- 文字：Echoes -->
    <span class="poem-en" style="top: 25%; left: 10%;">Echoes</span>
    <!-- マトリックス風文章：英語＋日本語、100行、生物的動き、Releases上部で消える -->
    <div class="matrix-text" style="top: 2%;" data-wave="0" data-speed="0.1">To transform the structured art of “music” into ambiguous particles...</div>
    <div class="matrix-text" style="top: 4%;" data-wave="5" data-speed="0.15">將「音樂」這種有結構的藝術轉化為記憶與空間的曖昧粒子...</div>
    <div class="matrix-text" style="top: 6%; left: 10%;" data-wave="10" data-speed="0.2">It—is neither “story” nor “emotion”. It is the sensation of fragments...</div>
    <div class="matrix-text" style="top: 8%; left: 20%;" data-wave="15" data-speed="0.25">它既非「故事」，也非「情感」。它是片段的感覺...</div>
    <div class="matrix-text" style="top: 10%;" data-wave="20" data-speed="0.3">In other words, I want to present as a work of art the very sensation...</div>
    <div class="matrix-text" style="top: 12%;" data-wave="25" data-speed="0.15">換句話說，我希望將「寂靜中微弱的模糊」這種感覺本身...</div>
    <div class="matrix-text" style="top: 14%; left: 30%;" data-wave="30" data-speed="0.2">Time is not a line but a layer, melody is not will but an accidental...</div>
    <div class="matrix-text" style="top: 16%; left: 40%;" data-wave="35" data-speed="0.25">時間不是線條，而是層次；旋律不是意志，而是偶然的玷污...</div>
    <div class="matrix-text" style="top: 18%;" data-wave="40" data-speed="0.1">I want to scoop up the contemporary “submerged sensation of being flooded...</div>
    <div class="matrix-text" style="top: 20%;" data-wave="45" data-speed="0.15">我想舀出當代「被聲音淹沒的淹沒感覺...</div>
    <div class="matrix-text" style="top: 22%; left: 50%;" data-wave="50" data-speed="0.2">If painters who painted light emerged in the Impressionist movement...</div>
    <div class="matrix-text" style="top: 24%; left: 60%;" data-wave="55" data-speed="0.25">如果印象派運動中出現了畫光的畫家...</div>
    <div class="matrix-text" style="top: 26%;" data-wave="60" data-speed="0.3">Songs with pauses can be a new form of ambient...</div>
    <div class="matrix-text" style="top: 28%;" data-wave="65" data-speed="0.1">有停頓的歌曲可以成為一種新的環境形式...</div>
    <div class="matrix-text" style="top: 30%; left: 70%;" data-wave="70" data-speed="0.15">One of the major differences between Western and Japanese music...</div>
    <div class="matrix-text" style="top: 32%; left: 80%;" data-wave="75" data-speed="0.2">西方音樂與日本音樂的主要差異之一，就是停頓的運用...</div>
    <div class="matrix-text" style="top: 34%;" data-wave="80" data-speed="0.25">Emotional sound waveforms in a limited environment...</div>
    <div class="matrix-text" style="top: 36%;" data-wave="85" data-speed="0.3">在有限的環境中，情感化的聲音波形...</div>
    <div class="matrix-text" style="top: 38%; left: 15%;" data-wave="90" data-speed="0.1">This huge album 1000 plateaux is of course borrowed from the title...</div>
    <div class="matrix-text" style="top: 40%; left: 25%;" data-wave="95" data-speed="0.15">這張巨大的專輯《1000 高原》當然是借用了 Gilles Deleuze...</div>
    <div class="matrix-text" style="top: 42%;" data-wave="100" data-speed="0.2">What is it about a mind made up of complex concepts of conflicts...</div>
    <div class="matrix-text" style="top: 44%;" data-wave="105" data-speed="0.25">在過去的兩年裡，我的心靈是由衝突和矛盾的複雜概念...</div>
    <div class="matrix-text" style="top: 46%; left: 35%;" data-wave="110" data-speed="0.3">What are the organs that cause the three major cravings?...</div>
    <div class="matrix-text" style="top: 48%; left: 45%;" data-wave="115" data-speed="0.1">引起三大渴望的器官是什麼？...</div>
    <div class="matrix-text" style="top: 50%;" data-wave="120" data-speed="0.15">The answer was here. The dynamism of the system itself is the core...</div>
    <div class="matrix-text" style="top: 52%;" data-wave="125" data-speed="0.2">答案就在這裡。系統本身的動力是思想的核心...</div>
    <div class="matrix-text" style="top: 54%; left: 55%;" data-wave="130" data-speed="0.25">In today's world dominated by mathematics, science and logic...</div>
    <div class="matrix-text" style="top: 56%; left: 65%;" data-wave="135" data-speed="0.3">在數學、科學和邏輯主導的現今世界...</div>
    <div class="matrix-text" style="top: 58%;" data-wave="140" data-speed="0.1">To transform the structured art of “music” into ambiguous particles...</div>
    <div class="matrix-text" style="top: 60%;" data-wave="145" data-speed="0.15">將「音樂」這種有結構的藝術轉化為記憶與空間的曖昧粒子...</div>
    <div class="matrix-text" style="top: 62%; left: 75%;" data-wave="0" data-speed="0.2">It is neither “story” nor “emotion”. It is the sensation of fragments...</div>
    <div class="matrix-text" style="top: 64%; left: 85%;" data-wave="5" data-speed="0.25">它既非「故事」，也非「情感」。它是片段的感覺...</div>
    <div class="matrix-text" style="top: 66%;" data-wave="10" data-speed="0.3">In other words, I want to present as a work of art the very sensation...</div>
    <div class="matrix-text" style="top: 68%;" data-wave="15" data-speed="0.1">換句話說，我希望將「寂靜中微弱的模糊」這種感覺本身...</div>
    <div class="matrix-text" style="top: 70%; left: 5%;" data-wave="20" data-speed="0.15">Time is not a line but a layer, melody is not will but an accidental...</div>
    <div class="matrix-text" style="top: 72%; left: 15%;" data-wave="25" data-speed="0.2">時間不是線條，而是層次；旋律不是意志，而是偶然的玷污...</div>
    <div class="matrix-text" style="top: 74%;" data-wave="30" data-speed="0.25">I want to scoop up the contemporary “submerged sensation of being flooded...</div>
    <div class="matrix-text" style="top: 76%;" data-wave="35" data-speed="0.3">我想舀出當代「被聲音淹沒的淹沒感覺...</div>
    <div class="matrix-text" style="top: 78%; left: 25%;" data-wave="40" data-speed="0.1">If painters who painted light emerged in the Impressionist movement...</div>
    <div class="matrix-text" style="top: 80%; left: 35%;" data-wave="45" data-speed="0.15">如果印象派運動中出現了畫光的畫家...</div>
    <div class="matrix-text" style="top: 82%;" data-wave="50" data-speed="0.2">Songs with pauses can be a new form of ambient...</div>
    <div class="matrix-text" style="top: 84%;" data-wave="55" data-speed="0.25">有停頓的歌曲可以成為一種新的環境形式...</div>
    <div class="matrix-text" style="top: 86%; left: 45%;" data-wave="60" data-speed="0.3">One of the major differences between Western and Japanese music...</div>
    <div class="matrix-text" style="top: 88%; left: 55%;" data-wave="65" data-speed="0.1">西方音樂與日本音樂的主要差異之一，就是停頓的運用...</div>
    <div class="matrix-text" style="top: 90%;" data-wave="70" data-speed="0.15">Emotional sound waveforms in a limited environment...</div>
    <div class="matrix-text" style="top: 92%;" data-wave="75" data-speed="0.2">在有限的環境中，情感化的聲音波形...</div>
    <div class="matrix-text" style="top: 94%; left: 65%;" data-wave="80" data-speed="0.25">This huge album 1000 plateaux is of course borrowed from the title...</div>
    <div class="matrix-text" style="top: 96%; left: 75%;" data-wave="85" data-speed="0.3">這張巨大的專輯《1000 高原》當然是借用了 Gilles Deleuze...</div>
    <div class="matrix-text" style="top: 98%;" data-wave="90" data-speed="0.1">What is it about a mind made up of complex concepts of conflicts...</div>
    <div class="matrix-text" style="top: 100%;" data-wave="95" data-speed="0.15">在過去的兩年裡，我的心靈是由衝突和矛盾的複雜概念...</div>
    <div class="matrix-text" style="top: 2%; left: 85%;" data-wave="100" data-speed="0.2">What are the organs that cause the three major cravings?...</div>
    <div class="matrix-text" style="top: 4%; left: 95%;" data-wave="105" data-speed="0.25">引起三大渴望的器官是什麼？...</div>
    <div class="matrix-text" style="top: 6%;" data-wave="110" data-speed="0.3">The answer was here. The dynamism of the system itself is the core...</div>
    <div class="matrix-text" style="top: 8%;" data-wave="115" data-speed="0.1">答案就在這裡。系統本身的動力是思想的核心...</div>
    <div class="matrix-text" style="top: 10%; left: 5%;" data-wave="120" data-speed="0.15">In today's world dominated by mathematics, science and logic...</div>
    <div class="matrix-text" style="top: 12%; left: 15%;" data-wave="125" data-speed="0.2">在數學、科學和邏輯主導的現今世界...</div>
    <div class="matrix-text" style="top: 14%;" data-wave="130" data-speed="0.25">To transform the structured art of “music” into ambiguous particles...</div>
    <div class="matrix-text" style="top: 16%;" data-wave="135" data-speed="0.3">將「音樂」這種有結構的藝術轉化為記憶與空間的曖昧粒子...</div>
    <div class="matrix-text" style="top: 18%; left: 25%;" data-wave="140" data-speed="0.1">It is neither “story” nor “emotion”. It is the sensation of fragments...</div>
    <div class="matrix-text" style="top: 20%; left: 35%;" data-wave="145" data-speed="0.15">它既非「故事」，也非「情感」。它是片段的感覺...</div>
    <div class="matrix-text" style="top: 22%;" data-wave="0" data-speed="0.2">In other words, I want to present as a work of art the very sensation...</div>
    <div class="matrix-text" style="top: 24%;" data-wave="5" data-speed="0.25">換句話說，我希望將「寂靜中微弱的模糊」這種感覺本身...</div>
    <div class="matrix-text" style="top: 26%; left: 45%;" data-wave="10" data-speed="0.3">Time is not a line but a layer, melody is not will but an accidental...</div>
    <div class="matrix-text" style="top: 28%; left: 55%;" data-wave="15" data-speed="0.1">時間不是線條，而是層次；旋律不是意志，而是偶然的玷污...</div>
    <div class="matrix-text" style="top: 30%;" data-wave="20" data-speed="0.15">I want to scoop up the contemporary “submerged sensation of being flooded...</div>
    <div class="matrix-text" style="top: 32%;" data-wave="25" data-speed="0.2">我想舀出當代「被聲音淹沒的淹沒感覺...</div>
    <div class="matrix-text" style="top: 34%; left: 65%;" data-wave="30" data-speed="0.25">If painters who painted light emerged in the Impressionist movement...</div>
    <div class="matrix-text" style="top: 36%; left: 75%;" data-wave="35" data-speed="0.3">如果印象派運動中出現了畫光的畫家...</div>
    <div class="matrix-text" style="top: 38%;" data-wave="40" data-speed="0.1">Songs with pauses can be a new form of ambient...</div>
    <div class="matrix-text" style="top: 40%;" data-wave="45" data-speed="0.15">有停頓的歌曲可以成為一種新的環境形式...</div>
    <div class="matrix-text" style="top: 42%; left: 85%;" data-wave="50" data-speed="0.2">One of the major differences between Western and Japanese music...</div>
    <div class="matrix-text" style="top: 44%; left: 95%;" data-wave="55" data-speed="0.25">西方音樂與日本音樂的主要差異之一，就是停頓的運用...</div>
    <div class="matrix-text" style="top: 46%;" data-wave="60" data-speed="0.3">Emotional sound waveforms in a limited environment...</div>
    <div class="matrix-text" style="top: 48%;" data-wave="65" data-speed="0.1">在有限的環境中，情感化的聲音波形...</div>
    <div class="matrix-text" style="top: 50%; left: 5%;" data-wave="70" data-speed="0.15">This huge album 1000 plateaux is of course borrowed from the title...</div>
    <div class="matrix-text" style="top: 52%; left: 15%;" data-wave="75" data-speed="0.2">這張巨大的專輯《1000 高原》當然是借用了 Gilles Deleuze...</div>
    <div class="matrix-text" style="top: 54%;" data-wave="80" data-speed="0.25">What is it about a mind made up of complex concepts of conflicts...</div>
    <div class="matrix-text" style="top: 56%;" data-wave="85" data-speed="0.3">在過去的兩年裡，我的心靈是由衝突和矛盾的複雜概念...</div>
    <div class="matrix-text" style="top: 58%; left: 25%;" data-wave="90" data-speed="0.1">What are the organs that cause the three major cravings?...</div>
    <div class="matrix-text" style="top: 60%; left: 35%;" data-wave="95" data-speed="0.15">引起三大渴望的器官是什麼？...</div>
    <div class="matrix-text" style="top: 62%;" data-wave="100" data-speed="0.2">The answer was here. The dynamism of the system itself is the core...</div>
    <div class="matrix-text" style="top: 64%;" data-wave="105" data-speed="0.25">答案就在這裡。系統本身的動力是思想的核心...</div>
    <div class="matrix-text" style="top: 66%; left: 45%;" data-wave="110" data-speed="0.3">In today's world dominated by mathematics, science and logic...</div>
    <div class="matrix-text" style="top: 68%; left: 55%;" data-wave="115" data-speed="0.1">在數學、科學和邏輯主導的現今世界...</div>
    <div class="matrix-text" style="top: 70%;" data-wave="120" data-speed="0.15">To transform the structured art of “music” into ambiguous particles...</div>
    <div class="matrix-text" style="top: 72%;" data-wave="125" data-speed="0.2">將「音樂」這種有結構的藝術轉化為記憶與空間的曖昧粒子...</div>
    <div class="matrix-text" style="top: 74%; left: 65%;" data-wave="130" data-speed="0.25">It is neither “story” nor “emotion”. It is the sensation of fragments...</div>
    <div class="matrix-text" style="top: 76%; left: 75%;" data-wave="135" data-speed="0.3">它既非「故事」，也非「情感」。它是片段的感覺...</div>
    <div class="matrix-text" style="top: 78%;" data-wave="140" data-speed="0.1">In other words, I want to present as a work of art the very sensation...</div>
    <div class="matrix-text" style="top: 80%;" data-wave="145" data-speed="0.15">換句話說，我希望將「寂靜中微弱的模糊」這種感覺本身...</div>
    <div class="matrix-text" style="top: 82%; left: 85%;" data-wave="0" data-speed="0.2">Time is not a line but a layer, melody is not will but an accidental...</div>
    <div class="matrix-text" style="top: 84%; left: 95%;" data-wave="5" data-speed="0.25">時間不是線條，而是層次；旋律不是意志，而是偶然的玷污...</div>
    <div class="matrix-text" style="top: 86%;" data-wave="10" data-speed="0.3">I want to scoop up the contemporary “submerged sensation of being flooded...</div>
    <div class="matrix-text" style="top: 88%;" data-wave="15" data-speed="0.1">我想舀出當代「被聲音淹沒的淹沒感覺...</div>
    <div class="matrix-text" style="top: 90%; left: 5%;" data-wave="20" data-speed="0.15">If painters who painted light emerged in the Impressionist movement...</div>
    <div class="matrix-text" style="top: 92%; left: 15%;" data-wave="25" data-speed="0.2">如果印象派運動中出現了畫光的畫家...</div>
    <div class="matrix-text" style="top: 94%;" data-wave="30" data-speed="0.25">Songs with pauses can be a new form of ambient...</div>
    <div class="matrix-text" style="top: 96%;" data-wave="35" data-speed="0.3">有停頓的歌曲可以成為一種新的環境形式...</div>
    <div class="matrix-text" style="top: 98%; left: 25%;" data-wave="40" data-speed="0.1">One of the major differences between Western and Japanese music...</div>
    <div class="matrix-text" style="top: 100%; left: 35%;" data-wave="45" data-speed="0.15">西方音樂與日本音樂的主要差異之一，就是停頓的運用...</div>
  </div>
  <section class="releases">
    <h2>Releases</h2>
    <div class="album-grid">
      <div class="album-item">
        <span>Play Mute Pause Theory (2024)</span>
        <div class="album-links">
          <a href="https://open.spotify.com/intl-ja/album/4tmlykgdRBQrBoF8wjHVnA" target="_blank">Spotify</a>
          <a href="https://music.apple.com/jp/album/play-mute-pause-theory/1735529796" target="_blank">Apple Music</a>
        </div>
      </div>
      <div class="album-item">
        <span>AMBITED (2023)</span>
        <div class="album-links">
          <a href="https://open.spotify.com/intl-ja/album/20mSF4BIfsx2Xeujgxjf10" target="_blank">Spotify</a>
          <a href="https://music.apple.com/jp/album/ambited/1683768835" target="_blank">Apple Music</a>
        </div>
      </div>
      <div class="album-item">
        <span>1000 Plateaux (2020)</span>
        <div class="album-links">
          <a href="https://open.spotify.com/intl-ja/album/7KvioL7aqlriuZQccAVyhK" target="_blank">Spotify</a>
          <a href="https://music.apple.com/jp/album/1000-plateaux/1531872097" target="_blank">Apple Music</a>
        </div>
      </div>
    </div>
  </section>
  <section class="sns-contact">
    <h2>Contact</h2>
    <div class="sns-links">
      <a href="https://www.instagram.com/hiiroissiki" target="_blank"><i class="fab fa-instagram"></i></a>
      <a href="https://music.apple.com/jp/artist/hiiro-issiki/1531872098" target="_blank"><i class="fab fa-apple"></i></a>
      <a href="https://open.spotify.com/intl-ja/artist/0liySOeMG87MDy1XdjqOLh" target="_blank"><i class="fab fa-spotify"></i></a>
      <a href="https://www.deezer.com/artist/107302752" target="_blank"><i class="fas fa-music"></i></a>
      <a href="https://soundcloud.com/hiiroissiki" target="_blank"><i class="fab fa-soundcloud"></i></a>
      <a href="https://www.discogs.com/ja/artist/8213001-Hiiro-Issiki" target="_blank"><i class="fas fa-record-vinyl"></i></a>
    </div>
    <div class="contact">
      <p>Contact: <a href="mailto:hiiroissiki@gmail.com">hiiroissiki@gmail.com</a></p>
    </div>
  </section>
  <script>
    const texts = document.querySelectorAll('.matrix-text');
    const releases = document.querySelector('.releases');
    const releasesTop = releases.offsetTop - 100; // Releases上部で消える
    texts.forEach(text => {
      let x = parseFloat(text.style.left || '0') * window.innerWidth / 100;
      let y = parseFloat(text.style.top) * window.innerHeight / 100;
      let wave = parseFloat(text.dataset.wave);
      let speed = parseFloat(text.dataset.speed);
      let angle = Math.random() * 2 * Math.PI; // ランダムな初期角度
      function move() {
        // 生物のようなランダムな動き
        angle += (Math.random() - 0.5) * 0.2; // 角度を揺らす
        x += Math.cos(angle) * speed * 10; // 不規則なx移動
        y += Math.sin(angle) * speed * 10; // 不規則なy移動
        // 波形歪み
        const offset = Math.sin(wave * 0.1) * 15;
        text.style.transform = `translate(${x}px, ${y + offset}px)`;
        wave += 0.2;
        // Releases上部で消える
        if (y > releasesTop) {
          text.style.opacity = '0';
        } else {
          text.style.opacity = '1';
        }
        // 画面外でリセット
        if (x < -text.offsetWidth || x > window.innerWidth || y < -text.offsetHeight || y > window.innerHeight) {
          x = Math.random() * window.innerWidth;
          y = -text.offsetHeight;
          angle = Math.random() * 2 * Math.PI;
          text.style.opacity = '1';
        }
        requestAnimationFrame(move);
      }
      move();
    });
  </script>
</body>
</html>## Hi there 👋

<!--
**Hiiroissiki/HiiroIssiki** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
