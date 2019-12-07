# worldwind
Working with NASA WorldWind project

## Setup apache-ant

### Download apache-ant-1.10.7-bin.zip

download from [here](https://ant.apache.org/bindownload.cgi)

On Windows machine

```sh
# On Windows machine
mkdir C:\apache

cd apache
unzip apache-ant-1.10.7-bin.zip
```
On Linux machine

```sh
# On Linux machine
mkdir ~/apache

cd ~/apache
unzip apache-ant-1.10.7-bin.zip
```

### Set environment
On Windows machine
```sh
# On Windows machine

set PATH=%PATH%;%ANT_HOME%\bin
```
On Linux machine
```sh
# On Linux machine
export ANT_HOME=/home/$USER/apache/apache-ant-1.10.7

export PATH=$PATH:$ANT_HOME/bin
```
## Get WorldWind and build it

### Clone WorldWindJava

```sh
mkdir ~/workspace_ww
cd ~/workspace_ww

git clone https://github.com/NASAWorldWind/WorldWindJava.git
```
### Build WorldWindJava

```sh
cd ~/workspace_ww/WorldWindJava

ant
```

## Try some examples

```sh
cd ~/workspace_ww/WorldWindJava

# Run default demo ( gov.nasa.worldwindx.examples.ApplicationTemplate )
run-demo.bash

# Run HelloWorldWind
run-demo.bash gov.nasa.worldwindx.examples.HelloWorldWind

# Run SimplestPossibleExample
run-demo.bash gov.nasa.worldwindx.examples.SimplestPossibleExample

# Run Graticule 
run-demo.bash gov.nasa.worldwindx.examples.Graticule 

# Run ViewControls 
run-demo.bash gov.nasa.worldwindx.examples.ViewControls 


```
