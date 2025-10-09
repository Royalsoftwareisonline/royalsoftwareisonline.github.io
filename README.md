
<head>
  <meta charset="UTF-8">
  <title>Video with Hints</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #cec5c5;
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }
    h1 {
      text-align: center;
    }
    video {
      width: 100%;
      max-height: 400px;
      margin-bottom: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    }
    .hint {
      margin: 10px 0;
      font-size: 18px;
    }
    .spoiler {
      background-color: black;
      color: black;
      border-radius: 4px;
      padding: 2px 6px;
      cursor: pointer;
      transition: color 0.2s ease, background-color 0.2s ease;
    }
    .spoiler.revealed {
      color: rgb(0, 0, 0);
      background-color: transparent;
    }
  </style>
</head>
<body>
  <h1>"(Ignore the thing above this btw)</h1>
  <h1>"A spectrogram is a visual representation of the spectrum of frequencies of a signal as it varies with time."</h1>

  <!-- Video Player -->
<video width="320" height="240" controls>
  <source src="Birthday_Hint_Video.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
<h1>"Only use hints if you NEED them. Start by downloading the video file.</h1>

  <!-- Hints -->
   <div class="hint">
    hint 1: <span class="spoiler">Something didn't sound right... I think Audacity may be your friend here.</span>
  </div>
  <div class="hint">
    hint 2: <span class="spoiler">I what those three dots next to the track name do...</span>
  </div>
  <div class="hint">
    hint 3: <span class="spoiler">One of the most common ways things are hidden in an image is by changing the brightness/contrast. Try playing with the "brightness" of the audio.</span>
  </div>
  <div class="hint">
    hint 4: <span class="spoiler">Try viewing the audio as a spectrogram, and then in Graphic EQ pulling all the sliders down until the text is revealed.</span>
  </div>

  <script>
    document.querySelectorAll('.spoiler').forEach(el => {
      el.addEventListener('click', () => {
        el.classList.add('revealed');
      });
    });
  </script>
</body>
</html>

