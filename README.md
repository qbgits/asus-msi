# asus-msi
# update
sudo dnf install kernel kernel-headers kernel-core kernel-debug kernel-debug-core kernel-debug-devel kernel-debug-modules kernel-debug-modules-extra kernel-devel kernel-modules kernel-modules-extra make automake gcc gcc-c++ kernel-devel git dkms dnf-utils wget unrar -y

sudo dnf update kernel kernel-headers kernel-core kernel-debug kernel-debug-core kernel-debug-devel kernel-debug-modules kernel-debug-modules-extra kernel-devel kernel-modules kernel-modules-extra make automake gcc gcc-c++ kernel-devel git dkms dnf-utils wget unrar -y

# Reboot
sudo shutdown -h now

# get repo:
git clone https://github.com/tomaspinho/rtl8821ce
cd rtl8821ce
chmod +x dkms-install.sh
chmod +x dkms-remove.sh

#Log out of Wayland Session and log into Xorg
# simply log out and then log in
# Open terminal.
sudo su
# Open terminal. Type sudo su (and then enter your password to get root access); you are now root.


# If you are in 'rtl8821ce' directory open terminal there.
cd rtl8821ce

# Run 'sudo ./dkms-install.sh' and wait for the process to complete.
sudo ./dkms-install.sh

# Now open settings and you can probably see a new section Wi-Fi is added.
# Turn on wifi and connect to your device.
