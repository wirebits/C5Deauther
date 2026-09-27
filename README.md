# 🛜C5Deauther
A tool that deauth 2.4GHz and 5GHz Wi-Fi networks via ESP32C5 on serial console.

# ✨Features
- Minimal Setup.
- Simply controlled by Serial Console.

# 📦Requirements
- `1` Waveshare ESP32-C5 N32R8 Development Board
- `1` Type-C USB Cable with data transfer support

>[!NOTE]
>Use those varient which contain atleast `4MB` flash memory.

# 🔧Install
1. Download `.bin` file from [here](url).
2. Download `esptool.exe` from [here](url).
3. Connect board by `UART` port to the computer.
4. Put both files in a folder.
5. Open `CMD` in that folder.
6. Type the following command to check `COM` port of that board:
```
mode
```
7. Type the following command to flash `.bin` file on the board:
```
esptool.exe --chip esp32c5 --baud 460800 --port COMx write_flash 0x0000 C5Deauther.bin
```
9. Replace `x` after the `COM` with the number show by `mode` command.
9. Hit Enter.
   - Wait for sometimes to flash.
10. Done!

# 📟Using Serial Console
1. Open Serial Console by click [here](https://wirebits.github.io/SerialConsole/).
2. Unplug and plug again board by `UART` port.
3. Click on `Connect` button.
   - It show a pop-up window and it has connect devices with port number.
   - Select the correct device.
   - Click on `Connect` button in pop-up window.
4. When it shows `Connected! Go On!` then your ESP32 Development Board is ready to use.
5. Press and release `EN` or `RST` button.
6. Type `help` to get available commands.
