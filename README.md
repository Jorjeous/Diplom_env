# Diplom_env
#Set up environment

sudo apt update
sudo apt install python3-dev python3-pip python3-venv

sudo apt install nvidia-cuda-toolkit
sudo apt install nvidia-cuda-dev

pip install wheel

pip3 install tensorflow
pip3 install Keras

#войти в папку LPCNet

./autohen.sh
./configure
make

./src/trainlpcnet.py Short_features.f32 Short_data.u8
