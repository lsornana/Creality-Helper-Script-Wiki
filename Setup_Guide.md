Great! Since you've already rooted your Creality K1C, let's proceed with installing the Creality Helper Script and setting up useful plugins. Here's a step-by-step guide:
Installing Creality Helper Script
SSH into your K1C using the following command:
text
ssh root@<your-printer-ip>
Enter your root password when prompted.
Clone the Helper Script repository:
text
git clone https://github.com/Guilouz/Creality-Helper-Script.git /usr/data/helper-script
Run the Helper Script:
text
sh /usr/data/helper-script/helper.sh
Installing Useful Plugins
Now that the Helper Script is installed, let's go through the install menu and set up useful items for your K1C:
1. Moonraker and Nginx
From the main menu, select "[Install]"
Choose "Moonraker and Nginx"
Follow the on-screen prompts to complete the installation
2. Web Interface (Fluidd or Mainsail)
From the [Install] menu, select either "Fluidd" or "Mainsail" (choose one)
Follow the installation prompts
3. Entware
From the [Install] menu, select "Entware"
Wait for the installation to complete
4. Klipper Adaptive Meshing & Purging (KAMP)
From the [Install] menu, choose "KAMP"
Follow the on-screen instructions
5. Crowsnest (for webcam support)
Select "Crowsnest" from the [Install] menu
Complete the installation process
6. Timelapse
Choose "Timelapse" from the [Install] menu
Follow the prompts to set it up
7. Telegram Bot
Select "Telegram Bot" from the [Install] menu
Follow the configuration steps, including setting up your Telegram bot token
8. Exclude Objects
Choose "Exclude Objects" from the [Install] menu
Complete the installation
9. Guppy Screen (optional)
If you want to replace the touch screen interface, select "Guppy Screen" from the [Install] menu
Follow the installation instructions
Post-Installation Steps
Exit the Helper Script
Restart your printer:
text
reboot
After reboot, access your new web interface by entering http://<your-printer-ip>:4408 (for Fluidd) or http://<your-printer-ip>:4409 (for Mainsail) in your browser2.
In the web interface, go to the "Machine" tab and check your printer.cfg file. Make sure all the newly installed components are properly configured.
If you installed KAMP, you'll need to add the necessary macros to your printer.cfg. Refer to the KAMP documentation for specific macro configurations.
For Timelapse, configure your settings in the web interface under the "Timelapse" tab.
If you installed the Telegram Bot, configure it using the instructions provided during installation.
Remember to test each new feature carefully and adjust configurations as needed for your specific K1C setup. If you encounter any issues, consult the Creality Helper Script documentation or community forums for troubleshooting18.
