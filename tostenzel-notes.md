- Note that (as written in the INSTALL.md) the program requires Python 3.7.
Hence, install `python3.7`, and `python3.7-dev` for installing from wheels. 

- For installing lapsolver during requirements installation, CMAKE must be installed beforehand with `sudo apt-get install cmake cmake-qt-gui 
`

- To create the virtualenv with python 3.7, type `python3.7 -m venv .py37-venv`

- After step 2.1 `pip3 install -r requirements.txt`, run `pip install numpy==1.21.6` in order to avoid numpy dimensions error during `python src/track.py`. The pre-specified numpy version is apparently too low.