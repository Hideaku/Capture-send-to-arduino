# Arduino 3D Cube and Serial Display

This project includes two main components:
1. **Arduino Code**: Renders a rotating 3D cube on an OLED display and handles incoming image data via serial.
2. **Python Script**: Captures the screen, processes the image, and sends it to the Arduino via serial.

## Arduino Code

**Libraries Required:**
- `Adafruit_GFX`
- `Adafruit_SSD1306`

**Features:**
- Draws a rotating 3D cube on a 128x64 OLED display.
- Displays incoming image data received via serial.

## Python Script

**Dependencies:**
- `opencv-python`
- `numpy`
- `mss`
- `pynput`
- `pyserial`

**Features:**
- Captures the screen.
- Processes the image (resize, threshold).
- Sends the image data to the Arduino over serial.

## How to Use

1. Upload the Arduino code to your Arduino board.
2. Run the Python script on your computer.
3. Press `*` on your keyboard to take scre
