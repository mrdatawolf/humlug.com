```bash
#!/usr/bin/env bash
#
# Meshtastic Serial Fix Script for Bazzite / Silverblue / Fedora
# --------------------------------------------------------------
# This script DOES NOT modify your system automatically.
# Instead, it documents the exact steps required to fix:
#   - Serial port access failures
#   - Missing dialout group
#   - ModemManager interference
#   - Flatpak Edge blocking Web Serial
#
# Run this script to *view* the commands and explanations.
# Copy/paste the ones you need.
#

echo "------------------------------------------------------------"
echo " Meshtastic Serial Troubleshooting Reference"
echo "------------------------------------------------------------"
echo

echo "1) Install Microsoft Edge (RPM version, NOT Flatpak)"
echo "# Bazzite requires the RPM version for Web Serial access."
echo "# This installs the repo + browser into the immutable image:"
echo "sudo rpm-ostree install https://packages.microsoft.com/yumrepos/edge/Packages/m/microsoft-edge-stable-146.0.3856.84-1.x86_64.rpm"
echo

echo "2) Remove Flatpak Edge if it exists (it cannot access serial ports)"
echo "flatpak uninstall com.microsoft.Edge"
echo

echo "3) Verify the Meshtastic device path"
echo "# Most Wio Tracker devices appear as /dev/ttyACM0"
echo "ls -l /dev/ttyACM*"
echo

echo "4) Ensure the dialout group exists"
echo "getent group dialout"
echo

echo "5) Manually add yourself to the dialout group"
echo "# On Bazzite/Silverblue, usermod may fail silently."
echo "# Editing /etc/group directly is the reliable method."
echo
echo "sudo nano /etc/group"
echo "# Add or modify the line to:"
echo "# dialout:x:18:YOURUSERNAME"
echo

echo "6) Restart your user session so group membership applies"
echo "# Reboot is NOT enough on Bazzite."
echo "loginctl terminate-user \$USER"
echo "# Then log back in normally."
echo

echo "7) Disable ModemManager (it grabs /dev/ttyACM0 and blocks Web Serial)"
echo "sudo systemctl stop ModemManager"
echo "sudo systemctl disable ModemManager"
echo

echo "8) Verify nothing else is holding the serial port"
echo "lsof /dev/ttyACM0"
echo

echo "9) Check dmesg for ACM/USB issues"
echo "dmesg | tail -n 40"
echo

echo "10) Launch Edge (RPM version) and test Web Serial"
echo "# Meshtastic Web → Connect → Serial → Select /dev/ttyACM0"
echo

echo "------------------------------------------------------------"
echo " Done. Follow the steps above to ensure stable Web Serial."
echo "------------------------------------------------------------"
```