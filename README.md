# Tools-<!DOCTYPE html><html lang="en"><head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Compress your images online with high-quality results. Fast, secure and free image compression tool by jasmindersingh28.github.io" />
  <meta name="keywords" content="image compression, online image compressor, reduce image size, compress jpg, compress png, web image optimization" />
  <meta name="author" content="Jasminder Singh" />
  <title>Image Compressor - jasmindersingh28.github.io</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }body {
  background: #f5f7fa;
  color: #333;
}

header {
  background: #4a90e2;
  padding: 20px;
  text-align: center;
  color: white;
}

header h1 {
  font-size: 2.5em;
  margin-bottom: 5px;
}

main {
  max-width: 800px;
  margin: 40px auto;
  background: white;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 10px;
  font-weight: bold;
}

input[type='file'],
select {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  background: #4a90e2;
  color: white;
  border: none;
  padding: 12px 25px;
  border-radius: 5px;
  font-size: 1em;
  cursor: pointer;
  transition: background 0.3s ease;
}

button:hover {
  background: #357ab8;
}

#preview {
  margin-top: 20px;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

img {
  max-width: 100%;
  border-radius: 8px;
}

footer {
  text-align: center;
  margin: 50px 0 20px;
  color: #777;
}

@media (max-width: 600px) {
  header h1 {
    font-size: 2em;
  }

  main {
    margin: 20px;
    padding: 20px;
  }
}

  </style>
</head><body>
  <header>
    <h1>Image Compressor</h1>
    <p>Reduce image size without losing quality</p>
  </header>  <main>
    <div class="form-group">
      <label for="imageUpload">Select an image:</label>
      <input type="file" id="imageUpload" accept="image/*" />
    </div><div class="form-group">
  <label for="compressionLevel">Choose Compression Level:</label>
  <select id="compressionLevel">
    <option value="0.9">Low (90%)</option>
    <option value="0.7">Medium (70%)</option>
    <option value="0.5">High (50%)</option>
  </select>
</div>

<button onclick="compressImage()">Compress Image</button>

<div id="preview"></div>

  </main>  <footer>
    &copy; 2025 jasmindersingh28.github.io | All rights reserved
  </footer>  <!-- Google AdSense Ad Unit -->  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXX"
    crossorigin="anonymous"></script><ins class="adsbygoogle"
style="display:block; text-align:center; margin-top: 20px;"
data-ad-client="ca-pub-XXXXXXXXXXXXXX"
data-ad-slot="1234567890"
data-ad-format="auto"
data-full-width-responsive="true"></ins>

  <script>
    (adsbygoogle = window.adsbygoogle || []).push({});
  </script>  <script>
    function compressImage() {
      const fileInput = document.getElementById('imageUpload');
      const compressionLevel = parseFloat(document.getElementById('compressionLevel').value);
      const preview = document.getElementById('preview');
      preview.innerHTML = '';

      const file = fileInput.files[0];
      if (!file) return alert('Please upload an image.');

      const reader = new FileReader();
      reader.onload = function (event) {
        const img = new Image();
        img.src = event.target.result;
        img.onload = function () {
          const canvas = document.createElement('canvas');
          const ctx = canvas.getContext('2d');

          canvas.width = img.width;
          canvas.height = img.height;
          ctx.drawImage(img, 0, 0);

          const compressedDataUrl = canvas.toDataURL('image/jpeg', compressionLevel);
          const compressedImg = document.createElement('img');
          compressedImg.src = compressedDataUrl;
          preview.appendChild(compressedImg);

          const downloadBtn = document.createElement('a');
          downloadBtn.href = compressedDataUrl;
          downloadBtn.download = 'compressed-image.jpg';
          downloadBtn.textContent = 'Download Compressed Image';
          downloadBtn.style.display = 'block';
          downloadBtn.style.marginTop = '15px';
          downloadBtn.style.textAlign = 'center';
          downloadBtn.style.fontWeight = 'bold';
          preview.appendChild(downloadBtn);
        };
      };
      reader.readAsDataURL(file);
    }
  </script></body></html>
