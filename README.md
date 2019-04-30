# iOS Fast Style Transfer
Simple IOS style transfer project.

## Getting started
This project was made for iOS 12.2.
In order to run this project you need:
- **Latest Xcode**
- **Torch**
Torch install all the dependencies via script. Conviniently, it also installs LuaJIT and LuaRocks
```
git clone https://github.com/torch/distro.git ~/torch --recursive
cd ~/torch; bash install-deps;
./install.sh
```
- **PyTorch 0.3.1**
You can install it via conda:
```
conda install pytorch=0.3.1 -c pytorch
```
- **Python 2.7**
- **torch2coreml** python package
```
pip install torch2coreml
```
### Preparing the .t7 models
There is a script that downloads the necessary t7 models.
```
bash fast_neural_style/models/download_style_transfer_models.sh
```
Then you can convert the t7 models to CoreML using the setup script
```
bash setup.sh
```
### Running the app
The Xcode project is located in /ios/ directory. Open it and Build for your device.
Enjoy!
