# Image-to-png.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image to PNG Converter | MultiTools</title>
    <meta name="description" content="Convert any image to PNG format online for free">
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Bootstrap Icons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.0/font/bootstrap-icons.css">
    <!-- Custom CSS -->
    <link href="../../../assets/css/style.css" rel="stylesheet">
    <link href="../../../assets/css/tools.css" rel="stylesheet">
</head>
<body>
    <!-- Header will be loaded dynamically -->
    <div id="header-container"></div>
    
    <main class="container mt-4">
        <div class="row">
            <div class="col-md-8">
                <h1>Image to PNG Converter</h1>
                <p class="lead">Convert any image (JPG, GIF, WEBP, etc.) to PNG format</p>
                
                <div class="tool-container p-4 border rounded">
                    <div class="mb-4">
                        <label for="file-input" class="form-label">Select an image file:</label>
                        <input type="file" id="file-input" class="form-control" accept="image/*">
                    </div>
                    
                    <div class="preview-area mb-4 text-center">
                        <img id="image-preview" class="img-fluid d-none" style="max-height: 300px;">
                        <div id="no-image" class="p-5 border rounded bg-light">
                            <i class="bi bi-image fs-1"></i>
                            <p class="mt-2">No image selected</p>
                        </div>
                    </div>
                    
                    <div class="options mb-4 d-none" id="options-section">
                        <h5>Conversion Options</h5>
                        <div class="form-check mb-2">
                            <input class="form-check-input" type="checkbox" id="transparency" checked>
                            <label class="form-check-label" for="transparency">Preserve transparency</label>
                        </div>
                        <div class="row">
                            <div class="col-md-6">
                                <label for="quality" class="form-label">Quality (1-100)</label>
                                <input type="range" class="form-range" min="1" max="100" value="90" id="quality">
                                <div class="text-center"><span id="quality-value">90</span>%</div>
                            </div>
                            <div class="col-md-6">
                                <label for="resize" class="form-label">Resize (optional)</label>
                                <div class="input-group">
                                    <input type="number" class="form-control" id="resize-width" placeholder="Width">
                                    <span class="input-group-text">x</span>
                                    <input type="number" class="form-control" id="resize-height" placeholder="Height">
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <button id="convert-btn" class="btn btn-primary" disabled>Convert to PNG</button>
                    <a id="download-btn" class="btn btn-success d-none ms-2">Download PNG</a>
                </div>
                
                <div class="mt-4">
                    <h3>How to use this tool</h3>
                    <ol>
                        <li>Click "Select an image file" or drag and drop an image</li>
                        <li>Adjust conversion options if needed</li>
                        <li>Click "Convert to PNG"</li>
                        <li>Download your converted PNG file</li>
                    </ol>
                </div>
            </div>
            
            <div class="col-md-4">
                <!-- Ad sidebar -->
                <div class="ad-sidebar sticky-top pt-4">
                    <div class="ad-placeholder mb-4">Advertisement</div>
                    
                    <div class="related-tools">
                        <h5>Related Tools</h5>
                        <ul class="list-group">
                            <li class="list-group-item"><a href="../image/image-to-jpg.html">Image to JPG Converter</a></li>
                            <li class="list-group-item"><a href="../image/image-resizer.html">Image Resizer</a></li>
                            <li class="list-group-item"><a href="../image/image-compressor.html">Image Compressor</a></li>
                            <li class="list-group-item"><a href="../image/webp-to-png.html">WEBP to PNG Converter</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </main>
    
    <!-- Footer will be loaded dynamically -->
    <div id="footer-container"></div>
    
    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <!-- Custom JS -->
    <script src="../../../assets/js/header-footer.js"></script>
    <script src="../../../assets/js/tools/image-to-png.js"></script>
</body>
</html>
