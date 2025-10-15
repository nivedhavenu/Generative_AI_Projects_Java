This is a simplified product image recognition demo that:

Scans the “src/main/resources/images” folder for JPG/JPEG/PNG files and processes images
Extracts basic visual features
Average RGB color values (normalized to 0-1)
Color ratios (red/green, blue/green, red/blue)
Brightness statistics
Edge density (using simple pixel difference)
Texture uniformity (from brightness histogram)
Makes “predictions” about what product is shown
Creates an annotated version of the image and saves results and modified images in output directory