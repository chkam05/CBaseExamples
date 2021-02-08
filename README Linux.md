# C++ Examples

## Setup C/C++ Development Environment for Ubuntu Linux

### Requirements:  

<br/>

1. Installing C/C++ Compiler and additional libraries.  

    ``` bash
    sudo apt-get install -y g++ cmake catkin libboost-all-dev doxygen
    ```

2. Installing Microsoft Visual Studio Code  

    * Enable Package Repository  

    ``` bash
    echo "deb [arch=amd64] http://packages.microsoft.com/repos/vscode stable main" | sudo tee /etc/apt/sources.list.d/vs-code.list
    ```

    * Import the package signing gpg key  

    ``` bash
    curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
    sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

    * Install Visual Studio Code  
    
    ``` bash
    sudo apt-get update
    sudo apt-get install -y code
    ```