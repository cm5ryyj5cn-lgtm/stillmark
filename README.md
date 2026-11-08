# Stillmark

Stillmark is a browser-based photo watermark studio. Add up to 20 photos, edit each one individually, and save watermarked exports directly to your device. Photos are processed locally in the browser and are not uploaded.

Select multiple placement points to add multiple watermarks. Choose a watermark in the list to edit its text and font independently, and drag each signature on the photo to reposition it. Size, opacity, color, and rotation are shared across signatures. Repeat-pattern mode uses the selected watermark and moves its tiled pattern as a whole.

Choose **Save as…** to select a filename and location. A single photo is saved as a PNG; multiple photos are saved together in a ZIP containing separate PNG exports. In browsers without a native save dialog, the export downloads using a suggested filename.

## Lightroom Classic workflow

Stillmark works with exported image files; it does not connect directly to the Lightroom Classic catalog or install as a Lightroom plugin.

1. In Lightroom Classic, select the photos and choose **File > Export**.
2. Export working copies as full-resolution JPEG or PNG into a temporary folder. Choose the color space and JPEG quality you normally use for delivery. Stillmark exports the finished images as PNG.
3. In Stillmark, add those exported files and edit the watermarks.
4. Choose **Save as…** and select where to save the PNG or ZIP export.
5. If you saved multiple photos in a ZIP, extract it. In Lightroom Classic, choose **File > Import Photos and Video**, select the PNG or extracted folder, and choose **Add** to keep the files there or **Copy** to place them in a managed folder.
6. If desired, select the imported PNGs and choose **Photo > Stacking > Group into Stack** to keep each watermarked derivative alongside its original.

The watermarked PNGs are flattened derivatives. Image metadata such as EXIF/GPS and Lightroom catalog edits, ratings, and keywords are not transferred; keep the originals in your catalog and back them up separately. Import the returned PNGs as new files rather than replacing the original photos.

No Python packages are required. Fonts load from Google Fonts when online; system fallbacks are used offline.
