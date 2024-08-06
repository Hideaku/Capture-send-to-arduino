# Arduino 3D Cube and Screen Capture

This project includes:
1. **Arduino Code**: Draws a rotating 3D cube on an OLED display and handles incoming image data via serial.
2. **Python Scripts**: Capture the screen and process images to send to the Arduino.

## Arduino Code

**File**: `arduino/cube_display.ino`

**Libraries Required:**
- `Adafruit_GFX`
- `Adafruit_SSD1306`

**Features:**
- Renders a rotating 3D cube on a 128x64 OLED display.
- Displays incoming image data received via serial communication.
- **Dynamic Display**: The 3D cube continues to render and rotate until image data is received via serial. When data is received, the display is cleared and updated with the new image.

## Python Scripts

**Directory**: `/python`

**Dependencies:**
- `opencv-python`
- `numpy`
- `mss`
- `pynput`
- `pyserial`

**Scripts:**

### `fast.py`

**Purpose**: Quickly process and send image data to the Arduino.

**Usage:**
1. Run the script to capture and send the screen image data.
2. Ensure the Arduino is connected and running the appropriate code.

### `slow.py`

**Purpose**: Includes screen capture functions with additional processing options.

**Usage:**
1. Run the script for advanced screen capture and processing.
2. Adjust settings as needed for different capture scenarios.

## How to Use

1. **Upload the Arduino Code**:
   - Open `cube_display.ino` in the Arduino IDE.
   - Upload it to your Arduino board.

2. **Run the Python Scripts**:
   - Ensure you have the required Python libraries installed.
   - Run `fast.py` or `slow.py` depending on your needs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
