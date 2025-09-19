# Task 2 - Tools Installation
Ensure existing packages are updated
```
sudo apt-get update
```

## YosysC
1. Clone the Yosys repository
```
git clone https://github.com/YosysHQ/yosys.git
cd yosys
```

2. Install make (skip if installed already)
```
sudo apt install make
```

3. Install neccessary development tools and libraries for Yosys
```
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
```

4. Choose gcc as compiler
```
make config-gcc
```

5. Download and initialise any required git submodules referenced by yosys
```
git submodule update --init
```

6. Compile yosys
```
make
```

7. Install yosys
```
sudo make install
```

#### Invoke yosys
```
yosys
```
<img width="625" alt="yosys" src="https://github.com/abhicmraja/vsd-rrstp/blob/49a5523d8e87d56c7ef70e9ece6dd9cc08a9ddde/assets/week0/yosys.png">

## Iverilog
Install iverilog
```
sudo apt-get install iverilog
```
#### Invoke iverilog
```
iverilog
```
<img width="625" alt="yosys" src="https://github.com/abhicmraja/vsd-rrstp/blob/49a5523d8e87d56c7ef70e9ece6dd9cc08a9ddde/assets/week0/iverilog.png">

## GTKWave
Install GTKWave
```
$ sudo apt install gtkwave
```

#### Invoke gtkwave
```
gtkwave
```
<img width="625" alt="yosys" src="https://github.com/abhicmraja/vsd-rrstp/blob/49a5523d8e87d56c7ef70e9ece6dd9cc08a9ddde/assets/week0/gtkwave.png">
GTKWave Display
<img width="625" alt="yosys" src="https://github.com/abhicmraja/vsd-rrstp/blob/49a5523d8e87d56c7ef70e9ece6dd9cc08a9ddde/assets/week0/gtkwave_display.png">
