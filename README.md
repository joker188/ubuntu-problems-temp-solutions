# ubuntu-problems-temp-solutions
wifi after suspend

wifi disconnecting after suspend problem, run this line:
sudo modprobe -r iwldvm && sudo modprobe iwldvm && sudo systemctl restart NetworkManager

Add an alias to bashrc:
alias wififix="sudo modprobe -r iwldvm && sudo modprobe iwldvm && sudo systemctl restart NetworkManager"
