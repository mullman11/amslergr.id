# Amsler Grid Reference Target

This website displays a **standardized Amsler grid** at the correct physical size (10 cm × 10 cm) for use as a reference target when capturing training images for the Lensometer app.

## Standard Specifications

According to ophthalmology standards:
- **Physical Size**: 10 cm × 10 cm (3.94 inches × 3.94 inches)
- **Grid Pattern**: 20×20 cells
- **Cell Size**: 5 mm × 5 mm each
- **Viewing Distance**: 30-38 cm (12-15 inches) from the eye
- **Visual Angle**: Each 5mm square subtends 1 degree at 30cm viewing distance

## Initial Setup & Calibration

### First Time Setup:

1. **Open** `index.html` in your web browser
2. **Calibration screen** will appear automatically
3. **Use a physical ruler** to measure the black line shown:
   - The line should measure exactly **10 cm** (or 3.94 inches)
   - Use the +/- buttons to adjust if needed
   - Press "Confirm" when the line measures exactly 10 cm
4. Your calibration is saved for future sessions

### Why Calibration Matters:

Different monitors have different pixel densities (DPI/PPI). CSS can't automatically know your monitor's exact physical dimensions, so calibration ensures:
- The grid displays at exactly 10 cm × 10 cm
- Consistent measurements across different setups
- Accurate lens distortion patterns for ML training

## Usage

### Option 1: Digital Display (For Training Data Collection)
1. Open `index.html` in your browser
2. Calibrate the grid on your monitor (first time only)
3. Press `F` for fullscreen mode (recommended)
4. Position eyeglass lens between iPhone camera and grid
5. Capture training photos through the lens

### Option 2: Printed Grid
1. Click "Print Grid" button on the website (or press `P`)
2. This opens the pre-generated `amsler-grid.pdf`
3. Print with settings: "Actual Size" or "100% scale"
4. Verify the printed grid measures exactly 10 cm × 10 cm using the calibration tools on page 2

**Note:** The PDF ensures consistent output across all printers and browsers. All users get the exact same printout.

## Keyboard Shortcuts

- `I` - Show usage instructions
- `F` - Enter fullscreen mode
- `P` - Open printable PDF
- `H` - Hide/show controls
- `C` - Open calibration screen
- `+` / `-` - Adjust grid size slightly (for monitor calibration)

## Grid Specifications

- **20×20 line grid** (21 lines total in each direction)
- Center lines are slightly thicker for reference
- Center dot for alignment
- High contrast for camera visibility
- Fixed physical dimensions (10 cm × 10 cm)

## Setup Tips

1. **Calibration**: Always calibrate on first use with each monitor
2. **Brightness**: Set monitor to maximum brightness for best contrast
3. **Distance**: Position monitor 12-18 inches from lens
4. **Angle**: Keep monitor perpendicular to camera view
5. **Lighting**: Use consistent ambient lighting, avoid glare on monitor
6. **Recalibration**: If you move to a different monitor, recalibrate

## Verification

To verify correct size:
1. Measure the grid with a physical ruler
2. Should be exactly 10 cm from left edge to right edge
3. Should be exactly 10 cm from top edge to bottom edge
4. If not exact, press `C` to recalibrate

## Technical Details

- Uses CSS physical units (`cm`) with calibration adjustment
- SVG-based grid for crisp rendering
- LocalStorage saves your calibration
- Pure HTML/CSS/JavaScript (no dependencies)
- Works offline
- Mobile-friendly (can use iPad/tablet as reference target)

## References

- Standard Amsler grid size: 10 cm × 10 cm
- Each cell: 5 mm × 5 mm
- Total cells: 20 × 20 = 400 cells
- Standard viewing distance: 30-38 cm
