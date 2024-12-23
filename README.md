# Setting-up-a-VM-for-completing-HTB-tasks
This is a short guide on creating a virtual working enviornment with a laptop running windows 11.

First off we need to ensure we meet the requirements to actually run a virtual machine on the laptop.
      Press the windows key and type 'command prompt' and open the command prompt application.  
      Then type 'systeminfo' this will then print details about the current computer what we are looking for is the section 'Hyper-V requirements'
      and we need to ensure that under 'VM Monitor Mode Extensions' it is labelled as yes.
      If this isnt the case then the issue can be remedied by installing a new CPU that supports VM monitor mode extensions.
      Attached is a copy of a command prompt using the 'systeminfo' command as an example
  ![image](https://github.com/user-attachments/assets/cf641c09-8496-412c-a34e-1c688d5b69f6)

Next we need to install OpenVPN connect from here: https://openvpn.net/client/  We also need to install Virtual box so we can actually host our VM heres the link: https://www.virtualbox.org/wiki/Downloads 
We arent done installing software yet we also need to download our OS. Im using Parrot OS, but HTB say on their website you can use other linux-based operating systems heres the links for parrot: https://parrotsec.org/download/
Next up, we need to download microsoft C++ redist 2019. Dont download the ARM64 version just the x86 and x64 versions we need these to actually be able to install virtual box on our computer Link: https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170

Now install OpenVPN, Virtual box and the microsoft redist packages.
Note, when installing virtual box you might get a pop up abount a missing python dependency you dont need to install this unless you plan on using python to control virtual box, it can be installed again at a later date so theres no harm in skipping for now, attached is the aforementioned pop up 
![image](https://github.com/user-attachments/assets/7c04b8c5-505b-4d20-83ad-4eec8d7d7214)

Now that virtual box is installed we can start our VM!
