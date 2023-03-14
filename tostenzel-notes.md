- The author writes that the **Pytorch and Torchvision versions in the installation.md are actually wrong!!!** "There is currently one issue with the INSTALL.md. It is supposed to read 2. Install PyTorch 1.7 and torchvision 0.8 from [here](https://pytorch.org/get-started/previous-versions/#v150). But there shouldnt be any failing packpaes when running the first pip install -r requirements.txt."

- Note that (as written in the INSTALL.md) the program requires Python 3.7.
Hence, install `python3.7`, and `python3.7-dev` for installing from wheels. 

- For installing lapsolver during requirements installation, CMAKE must be installed beforehand with `sudo apt-get install cmake cmake-qt-gui`.

- To create the virtualenv with python 3.7, type `python3.7 -m venv .py37-venv`.

- After step 2.1 `pip3 install -r requirements.txt`, run `pip install numpy==1.21.6` in order to avoid numpy dimensions error during `python src/track.py`. The pre-specified numpy version is apparently too low.

- Torchvision 0.8 does not work, therefore I use a higher one. It is best to use the highest ..X number because its always backward compatible.

- My best guess for now is `pip install torch==1.7.1+cu110 torchvision==0.8.2+cu110 torchaudio==0.7.2 -f https://download.pytorch.org/whl/torch_stable.html`.

- It is hard to cleanly uninstall `MultiScaleDeformableAttention`.

