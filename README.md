# Tools-<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Free online image compressor to reduce PNG and JPG file size without losing quality. Fast, efficient, and SEO optimized.">
  <meta name="keywords" content="Online Image Compressor, Free PNG & JPG Compression, Compress Images without Losing Quality, Fast Image Size Reducer, Web-based Image Optimization Tool">
  <meta name="author" content="Jasminder Singh">
  <meta property="og:title" content="Online Image Compressor">
  <meta property="og:description" content="Compress PNG and JPG images online for free. SEO optimized and responsive.">
  <meta property="og:url" content="https://jasmindersingh28.github.io">
  <meta property="og:type" content="website">
  <meta name="twitter:card" content="summary_large_image">
  <link rel="canonical" href="https://jasmindersingh28.github.io">
  <link rel="icon" href="favicon.ico" type="image/x-icon">
  <title>Online Image Compressor - Compress PNG & JPG</title>
  <script src="https://cdn.jsdelivr.net/npm/browser-image-compression@latest/dist/browser-image-compression.js"></script>
  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js" crossorigin="anonymous"></script>
  <style>
    body {
      font-family: sans-serif;
    }
    .hidden { display: none; }
  </style>
  <script>
    (adsbygoogle = window.adsbygoogle || []).push({});
  </script>
  <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebSite",
      "name": "Online Image Compressor",
      "url": "https://jasmindersingh28.github.io",
      "description": "Compress PNG and JPG images online without losing quality. Fast and free."
    }
  </script>
  <script>
    async function compressImage(file) {
      const options = {
        maxSizeMB: 1,
        maxWidthOrHeight: 1024,
        useWebWorker: true
      };
      try {
        const compressedFile = await imageCompression(file, options);
        const originalSize = (file.size / 1024).toFixed(2);
        const compressedSize = (compressedFile.size / 1024).toFixed(2);

        document.getElementById('results').innerHTML = `
          <p>Original Size: ${originalSize} KB</p>
          <p>Compressed Size: ${compressedSize} KB</p>
          <a download="compressed-${file.name}" href="${URL.createObjectURL(compressedFile)}">Download Compressed Image</a>
        `;
      } catch (error) {
        alert('Compression failed: ' + error.message);
      }
    }

    function handleFileInput(event) {
      const file = event.target.files[0];
      if (file && (file.type === 'image/jpeg' || file.type === 'image/png')) {
        compressImage(file);
      } else {
        alert('Please upload a valid PNG or JPG image.');
      }
    }
  </script>
</head>

<body class="bg-gray-100 text-gray-900">
  <header class="p-6 bg-blue-600 text-white text-center shadow-lg">
    <h1 class="text-2xl font-bold">Online Image Compressor</h1>
    <p class="text-sm">Compress PNG & JPG images online for free without losing quality.</p>
  </header>

  <main class="max-w-2xl mx-auto p-6 mt-6 bg-white rounded-2xl shadow-md">
    <div class="mb-4">
      <label for="imageInput" class="block text-lg font-semibold mb-2">Upload an image:</label>
      <input id="imageInput" type="file" accept="image/png, image/jpeg" class="w-full p-2 border border-gray-300 rounded" onchange="handleFileInput(event)" />
    </div>
    <div id="results" class="mt-4 text-sm"></div>
  </main>

  <div class="my-6 text-center">
    <ins class="adsbygoogle"
         style="display:block"
         data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
         data-ad-slot="YYYYYYYYYY"
         data-ad-format="auto"
         data-full-width-responsive="true"></ins>
    <script>
      (adsbygoogle = window.adsbygoogle || []).push({});
    </script>
  </div>

  <footer class="mt-10 text-center p-4 text-sm text-gray-500">
    &copy; 2025 <a href="https://github.com/jasmindersingh28" class="text-blue-500">Jasminder Singh</a> | All rights reserved.
  </footer>
</body>

</html>
