/Tools-<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Primary Meta Tags -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Image to PDF Converter | Convert JPG, PNG to PDF Online</title>
    <meta name="description" content="Convert multiple images to PDF online for free. No registration needed. Supports JPG, PNG, GIF, WEBP. Fast, secure, and works on all devices.">
    <meta name="keywords" content="image to pdf, jpg to pdf, png to pdf, convert images to pdf, free online pdf converter, image converter, online tools">
    <meta name="author" content="Jasminder Singh">
    
    <!-- Open Graph / Facebook Meta Tags -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://jasmindersingh28.github.io/Tools-/images-to-pdf/">
    <meta property="og:title" content="Free Image to PDF Converter | Convert JPG, PNG to PDF Online">
    <meta property="og:description" content="Convert multiple images to PDF online for free. No registration needed. Supports JPG, PNG, GIF, WEBP.">
    <meta property="og:image" content="https://jasmindersingh28.github.io/Tools-/images-to-pdf/assets/social-preview.jpg">
    
    <!-- Twitter Meta Tags -->
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:url" content="https://jasmindersingh28.github.io/Tools-/images-to-pdf/">
    <meta name="twitter:title" content="Free Image to PDF Converter | Convert JPG, PNG to PDF Online">
    <meta name="twitter:description" content="Convert multiple images to PDF online for free. No registration needed. Supports JPG, PNG, GIF, WEBP.">
    <meta name="twitter:image" content="https://jasmindersingh28.github.io/Tools-/images-to-pdf/assets/social-preview.jpg">
    
    <!-- Canonical URL -->
    <link rel="canonical" href="https://jasmindersingh28.github.io/Tools-/images-to-pdf/">
    
    <!-- Favicon -->
    <link rel="icon" href="assets/favicon.ico" type="image/x-icon">
    <link rel="apple-touch-icon" href="assets/apple-touch-icon.png">
    
    <!-- CSS -->
    <style>
        :root {
            --primary-color: #4a6bff;
            --secondary-color: #f8f9fa;
            --accent-color: #ff6b6b;
            --text-color: #333;
            --light-text: #666;
            --border-color: #ddd;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --border-radius: 8px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f5f7ff;
            color: var(--text-color);
            line-height: 1.6;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), #6a5acd);
            color: white;
            padding: 2rem 0;
            text-align: center;
            margin-bottom: 2rem;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        .converter-box {
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 2rem;
            margin-bottom: 2rem;
        }

        .upload-area {
            border: 2px dashed var(--border-color);
            border-radius: var(--border-radius);
            padding: 3rem 1rem;
            text-align: center;
            margin-bottom: 2rem;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .upload-area:hover, .upload-area.dragover {
            border-color: var(--primary-color);
            background-color: rgba(74, 107, 255, 0.05);
        }

        .upload-area i {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }

        .upload-area h3 {
            margin-bottom: 0.5rem;
            color: var(--text-color);
        }

        .upload-area p {
            color: var(--light-text);
            margin-bottom: 1rem;
        }

        .formats {
            font-size: 0.9rem;
            color: var(--light-text);
        }

        .btn {
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: var(--border-radius);
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }

        .btn i {
            font-size: 1rem;
        }

        .btn.primary {
            background-color: var(--primary-color);
            color: white;
        }

        .btn.primary:hover {
            background-color: #3a5bef;
            transform: translateY(-2px);
        }

        .btn.secondary {
            background-color: var(--secondary-color);
            color: var(--text-color);
        }

        .btn.secondary:hover {
            background-color: #e9ecef;
        }

        .options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .option {
            display: flex;
            flex-direction: column;
        }

        .option label {
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--text-color);
        }

        .option input, .option select {
            padding: 0.8rem;
            border: 1px solid var(--border-color);
            border-radius: var(--border-radius);
            font-size: 1rem;
        }

        .preview {
            margin-bottom: 2rem;
        }

        .preview h3 {
            margin-bottom: 1rem;
        }

        .image-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 1rem;
        }

        .image-item {
            position: relative;
            border: 1px solid var(--border-color);
            border-radius: var(--border-radius);
            overflow: hidden;
            height: 150px;
        }

        .image-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .image-item .remove-btn {
            position: absolute;
            top: 0.5rem;
            right: 0.5rem;
            background-color: var(--accent-color);
            color: white;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            border: none;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .image-item:hover .remove-btn {
            opacity: 1;
        }

        .actions {
            display: flex;
            justify-content: space-between;
        }

        .how-to-use, .features {
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 2rem;
            margin-bottom: 2rem;
        }

        .how-to-use h2, .features h2 {
            margin-bottom: 1.5rem;
            text-align: center;
            color: var(--primary-color);
        }

        .how-to-use ol {
            padding-left: 1.5rem;
        }

        .how-to-use li {
            margin-bottom: 0.5rem;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .feature {
            text-align: center;
            padding: 1.5rem;
            border-radius: var(--border-radius);
            transition: transform 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-5px);
        }

        .feature i {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }

        .feature h3 {
            margin-bottom: 0.5rem;
            color: var(--text-color);
        }

        .feature p {
            color: var(--light-text);
            font-size: 0.95rem;
        }

        .ad-container {
            margin: 2rem 0;
            text-align: center;
        }

        footer {
            background-color: var(--text-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        footer p {
            margin-bottom: 1rem;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
        }

        .footer-links a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s ease;
        }

        .footer-links a:hover {
            opacity: 0.8;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }

            .options {
                grid-template-columns: 1fr;
            }

            .actions {
                flex-direction: column;
                gap: 1rem;
            }

            .btn {
                width: 100%;
                justify-content: center;
            }

            .image-list {
                grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            }

            .feature-grid {
                grid-template-columns: 1fr;
            }

            .footer-links {
                flex-direction: column;
                gap: 0.5rem;
            }
        }

        /* Schema.org structured data */
        .sr-only {
            position: absolute;
            width: 1px;
            height: 1px;
            padding: 0;
            margin: -1px;
            overflow: hidden;
            clip: rect(0, 0, 0, 0);
            white-space: nowrap;
            border-width: 0;
        }
    </style>
    
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- AdSense -->
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_ADSENSE_ID" crossorigin="anonymous"></script>
    
    <!-- Schema.org markup for Google -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebApplication",
      "name": "Image to PDF Converter",
      "url": "https://jasmindersingh28.github.io/Tools-/images-to-pdf/",
      "description": "Free online tool to convert multiple images to a single PDF file. No registration required.",
      "applicationCategory": "UtilityApplication",
      "operatingSystem": "Any",
      "offers": {
        "@type": "Offer",
        "price": "0",
        "priceCurrency": "USD"
      },
      "creator": {
        "@type": "Person",
        "name": "Jasminder Singh"
      }
    }
    </script>
</head>
<body>
    <header>
        <div class="container">
            <h1><i class="fas fa-file-pdf"></i> Image to PDF Converter</h1>
            <p>Convert multiple images to a single PDF file quickly and easily</p>
        </div>
    </header>

    <main class="container">
        <div class="ad-container">
            <!-- AdSense Banner Ad -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="YOUR_AD_SLOT_ID"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>

        <div class="converter-box">
            <div class="upload-area" id="dropArea">
                <i class="fas fa-cloud-upload-alt"></i>
                <h3>Drag & Drop Images Here</h3>
                <p>or</p>
                <button class="btn" id="selectFiles">Select Images</button>
                <input type="file" id="fileInput" accept="image/*" multiple style="display: none;">
                <p class="formats">Supports: JPG, PNG, GIF, WEBP</p>
            </div>

            <div class="options">
                <div class="option">
                    <label for="pdfName">PDF Name:</label>
                    <input type="text" id="pdfName" placeholder="output.pdf">
                </div>
                <div class="option">
                    <label for="pageSize">Page Size:</label>
                    <select id="pageSize">
                        <option value="a4">A4</option>
                        <option value="letter">Letter</option>
                        <option value="legal">Legal</option>
                        <option value="fit">Fit to Image</option>
                    </select>
                </div>
                <div class="option">
                    <label for="pageOrientation">Orientation:</label>
                    <select id="pageOrientation">
                        <option value="portrait">Portrait</option>
                        <option value="landscape">Landscape</option>
                    </select>
                </div>
                <div class="option">
                    <label for="margin">Margin (mm):</label>
                    <input type="number" id="margin" value="10" min="0" max="50">
                </div>
            </div>

            <div class="preview" id="previewContainer">
                <h3>Selected Images (0)</h3>
                <div class="image-list" id="imageList"></div>
            </div>

            <div class="actions">
                <button class="btn secondary" id="clearAll">Clear All</button>
                <button class="btn primary" id="convertBtn" disabled>
                    <i class="fas fa-file-pdf"></i> Convert to PDF
                </button>
            </div>
        </div>

        <div class="ad-container">
            <!-- AdSense Banner Ad -->
            <ins class="adsbygoogle"
                 style="display:block"
                 data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                 data-ad-slot="YOUR_AD_SLOT_ID"
                 data-ad-format="auto"
                 data-full-width-responsive="true"></ins>
            <script>
                 (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>

        <div class="how-to-use">
            <h2>How to Convert Images to PDF</h2>
            <ol>
                <li>Select images or drag & drop them into the upload area</li>
                <li>Adjust PDF settings if needed (name, page size, etc.)</li>
                <li>Click "Convert to PDF" button</li>
                <li>Download your PDF file when ready</li>
            </ol>
        </div>

        <div class="features">
            <h2>Why Use Our Image to PDF Converter?</h2>
            <div class="feature-grid">
                <div class="feature">
                    <i class="fas fa-lock"></i>
                    <h3>Secure</h3>
                    <p>All processing happens in your browser. Your images never leave your device.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-bolt"></i>
                    <h3>Fast</h3>
                    <p>Convert multiple images to PDF in seconds with our optimized tool.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-cogs"></i>
                    <h3>Customizable</h3>
                    <p>Adjust page size, orientation, and margins to your needs.</p>
                </div>
                <div class="feature">
                    <i class="fas fa-dollar-sign"></i>
                    <h3>Free</h3>
                    <p>No hidden charges or subscriptions. Completely free to use.</p>
                </div>
            </div>
        </div>
        
        <!-- FAQ Schema -->
        <div class="sr-only" itemscope itemtype="https://schema.org/FAQPage">
            <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question">
                <h3 itemprop="name">Is this Image to PDF converter free to use?</h3>
                <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
                    <div itemprop="text">Yes, our Image to PDF converter is completely free to use with no hidden charges.</div>
                </div>
            </div>
            <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question">
                <h3 itemprop="name">What image formats are supported?</h3>
                <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
                    <div itemprop="text">We support JPG, PNG, GIF, and WEBP image formats.</div>
                </div>
            </div>
            <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question">
                <h3 itemprop="name">Are my images uploaded to a server?</h3>
                <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
                    <div itemprop="text">No, all processing happens in your browser. Your images never leave your device.</div>
                </div>
            </div>
        </div>
    </main>

    <footer>
        <div class="container">
            <p>&copy; <span id="currentYear"></span> Image to PDF Converter. Part of <a href="https://github.com/jasmindersingh28/Tools-">Tools Collection</a>.</p>
            <div class="footer-links">
                <a href="privacy.html">Privacy Policy</a>
                <a href="terms.html">Terms of Service</a>
                <a href="https://github.com/jasmindersingh28/Tools-/issues">Report an Issue</a>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script>
        // Wait for the DOM to be fully loaded
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year in footer
            document.getElementById('currentYear').textContent = new Date().getFullYear();
            
            // Get DOM elements
            const dropArea = document.getElementById('dropArea');
            const fileInput = document.getElementById('fileInput');
            const selectFilesBtn = document.getElementById('selectFiles');
            const previewContainer = document.getElementById('previewContainer');
            const imageList = document.getElementById('imageList');
            const clearAllBtn = document.getElementById('clearAll');
            const convertBtn = document.getElementById('convertBtn');
            const pdfNameInput = document.getElementById('pdfName');
            const pageSizeSelect = document.getElementById('pageSize');
            const pageOrientationSelect = document.getElementById('pageOrientation');
            const marginInput = document.getElementById('margin');
            
            let files = [];
            
            // Initialize jsPDF
            const { jsPDF } = window.jspdf;
            
            // Event listeners
            selectFilesBtn.addEventListener('click', () => fileInput.click());
            fileInput.addEventListener('change', handleFileSelect);
            clearAllBtn.addEventListener('click', clearAllFiles);
            convertBtn.addEventListener('click', convertToPDF);
            
            // Drag and drop events
            ['dragenter', 'dragover', 'dragleave', 'drop'].forEach(eventName => {
                dropArea.addEventListener(eventName, preventDefaults, false);
            });
            
            function preventDefaults(e) {
                e.preventDefault();
                e.stopPropagation();
            }
            
            ['dragenter', 'dragover'].forEach(eventName => {
                dropArea.addEventListener(eventName, highlight, false);
            });
            
            ['dragleave', 'drop'].forEach(eventName => {
                dropArea.addEventListener(eventName, unhighlight, false);
            });
            
            function highlight() {
                dropArea.classList.add('dragover');
            }
            
            function unhighlight() {
                dropArea.classList.remove('dragover');
            }
            
            dropArea.addEventListener('drop', handleDrop, false);
            
            function handleDrop(e) {
                const dt = e.dataTransfer;
                const newFiles = dt.files;
                handleFiles(newFiles);
            }
            
            function handleFileSelect(e) {
                const newFiles = e.target.files;
                handleFiles(newFiles);
            }
            
            function handleFiles(newFiles) {
                // Filter only image files
                const imageFiles = Array.from(newFiles).filter(file => 
                    file.type.match('image.*')
                );
                
                if (imageFiles.length === 0) {
                    alert('Please select only image files (JPG, PNG, GIF, WEBP).');
                    return;
                }
                
                files = [...files, ...imageFiles];
                updatePreview();
                fileInput.value = ''; // Reset file input
            }
            
            function updatePreview() {
                // Clear previous preview
                imageList.innerHTML = '';
                
                if (files.length === 0) {
                    previewContainer.style.display = 'none';
                    convertBtn.disabled = true;
                    return;
                }
                
                previewContainer.style.display = 'block';
                convertBtn.disabled = false;
                
                // Update count in heading
                const heading = previewContainer.querySelector('h3');
                heading.textContent = `Selected Images (${files.length})`;
                
                // Create preview for each file
                files.forEach((file, index) => {
                    const reader = new FileReader();
                    
                    reader.onload = function(e) {
                        const imageItem = document.createElement('div');
                        imageItem.className = 'image-item';
                        
                        const img = document.createElement('img');
                        img.src = e.target.result;
                        img.alt = file.name;
                        
                        const removeBtn = document.createElement('button');
                        removeBtn.className = 'remove-btn';
                        removeBtn.innerHTML = '<i class="fas fa-times"></i>';
                        removeBtn.title = 'Remove image';
                        removeBtn.addEventListener('click', (e) => {
                            e.stopPropagation();
                            removeFile(index);
                        });
                        
                        imageItem.appendChild(img);
                        imageItem.appendChild(removeBtn);
                        imageList.appendChild(imageItem);
                    };
                    
                    reader.readAsDataURL(file);
                });
            }
            
            function removeFile(index) {
                files.splice(index, 1);
                updatePreview();
            }
            
            function clearAllFiles() {
                files = [];
                updatePreview();
            }
            
            async function convertToPDF() {
                if (files.length === 0) return;
                
                convertBtn.disabled = true;
                convertBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Processing...';
                
                try {
                    // Create PDF
                    const pdf = new jsPDF({
                        orientation: pageOrientationSelect.value,
                        unit: 'mm'
                    });
                    
                    // Set PDF name
                    let pdfName = pdfNameInput.value.trim();
                    if (!pdfName) pdfName = 'output.pdf';
                    if (!pdfName.endsWith('.pdf')) pdfName += '.pdf';
                    
                    // Process each image
                    for (let i = 0; i < files.length; i++) {
                        const file = files[i];
                        const imgData = await readFileAsDataURL(file);
                        
                        // Add new page for each image after the first one
                        if (i > 0) {
                            pdf.addPage();
                        }
                        
                        // Get image dimensions
                        const img = await loadImage(imgData);
                        let imgWidth = img.width;
                        let imgHeight = img.height;
                        
                        // Calculate dimensions based on page size
                        let pageWidth, pageHeight;
                        const margin = parseInt(marginInput.value);
                        
                        switch (pageSizeSelect.value) {
                            case 'a4':
                                pageWidth = 210 - margin * 2;
                                pageHeight = 297 - margin * 2;
                                break;
                            case 'letter':
                                pageWidth = 216 - margin * 2;
                                pageHeight = 279 - margin * 2;
                                break;
                            case 'legal':
                                pageWidth = 216 - margin * 2;
                                pageHeight = 356 - margin * 2;
                                break;
                            case 'fit':
                                pageWidth = imgWidth;
                                pageHeight = imgHeight;
                                break;
                            default:
                                pageWidth = 210 - margin * 2;
                                pageHeight = 297 - margin * 2;
                        }
                        
                        // Calculate aspect ratio
                        const imgAspectRatio = imgWidth / imgHeight;
                        let displayWidth, displayHeight;
                        
                        if (imgAspectRatio > 1) {
                            // Landscape image
                            displayWidth = pageWidth;
                            displayHeight = pageWidth / imgAspectRatio;
                            
                            if (displayHeight > pageHeight) {
                                displayHeight = pageHeight;
                                displayWidth = pageHeight * imgAspectRatio;
                            }
                        } else {
                            // Portrait or square image
                            displayHeight = pageHeight;
                            displayWidth = pageHeight * imgAspectRatio;
                            
                            if (displayWidth > pageWidth) {
                                displayWidth = pageWidth;
                                displayHeight = pageWidth / imgAspectRatio;
                            }
                        }
                        
                        // Add image to PDF
                        pdf.addImage(imgData, 'JPEG', margin, margin, displayWidth, displayHeight);
                    }
                    
                    // Save PDF
                    pdf.save(pdfName);
                    
                    // Track conversion in Google Analytics (if you have it)
                    if (typeof gtag !== 'undefined') {
                        gtag('event', 'conversion', {
                            'event_category': 'Tools',
                            'event_label': 'Image to PDF Conversion',
                            'value': files.length
                        });
                    }
                    
                } catch (error) {
                    console.error('Error converting to PDF:', error);
                    alert('An error occurred while converting to PDF. Please try again.');
                } finally {
                    convertBtn.disabled = false;
                    convertBtn.innerHTML = '<i class="fas fa-file-pdf"></i> Convert to PDF';
                }
            }
            
            function readFileAsDataURL(file) {
                return new Promise((resolve, reject) => {
                    const reader = new FileReader();
                    reader.onload = () => resolve(reader.result);
                    reader.onerror = reject;
                    reader.readAsDataURL(file);
                });
            }
            
            function loadImage(src) {
                return new Promise((resolve, reject) => {
                    const img = new Image();
                    img.onload = () => resolve(img);
                    img.onerror = reject;
                    img.src = src;
                });
            }
            
            // Initialize with current date for default PDF name
            const today = new Date();
            const dateString = `${today.getFullYear()}-${today.getMonth()+1}-${today.getDate()}`;
            pdfNameInput.value = `images-${dateString}.pdf`;
        });
    </script>
</body>
</html>
