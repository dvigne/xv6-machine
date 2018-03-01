![Florida Polytechnic University](https://floridapoly.edu/wp-content/themes/floridapolytechnic/images/home_logo.png)
# XV6 Virtual Machine Local Development Environment
## Operating System Concepts

### Required Software
In order to run the local development box, both Vagrant and Virtual Box are required. You may find the downloads available below.
1. Virtualbox
  * https://www.virtualbox.org/wiki/Downloads
2. Vagrant
  * https://vagrantup.com
3. Git SCM
  * https://git-scm.com/downloads

### Cloning the Repository
In order to get the configuration files required you must either clone this repository or download the zip file from above,

To clone the repository use:
```
git clone https://github.com/dvigne/xv6-machine.git && cd xv6-machine
```

### Configuring the box
Once you have cloned the repository there will be a `Vagrantfile` for configuring the virtual machine and `Code` folder that contains a fresh, working copy of the XV6 operating system.

To run the virtual machine, you must first download the image using the command below:
```
vagrant box add dvigne/xv6-machine
```
### Turning on the Lights
After you have the Vagrant Box Downloaded and shared folders configured go ahead and turn the virtual machine on with:
```
vagrant up
```
and then connect with:
```
vagrant ssh
```
### Profit
After performing the above, you should have access to a shared folder named `Code` located at the root of the Vagrant Box. You can find the path of the Vagrant folder by typing either `cd` for Windows or `pwd` for Mac/Linux. As mentioned previously, this contains a clean, working copy of xv6 for you to modify as needed. This shared folder structure allows you to edit in your favorite text editor and your changes will be reflected within the virtual machine to compile and test. Your synced files are located within the virtual machine at `/home/vagrant/Code`.

Happy coding! :heart:
