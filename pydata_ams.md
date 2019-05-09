$ conda create -n pydata-ams
$ conda activate pydata-ams
$ conda install numpy dask jupyterlab
$ # If you have a NVIDIA GPU. Needs CUDA installed.
$ # CuPy 6.0.0 will be out soon, then conda-installable.
$ pip install --pre cupy-cuda100  # or cupy-90 for CUDA 9

$ python -c "import numpy; print(numpy.__version__)"
1.16.3
$ python -c "import cupy; print(cupy.__version__)"
6.0.0rc1
$ python -c "import dask; print(dask.__version__)"
1.2.0

$ export NUMPY_EXPERIMENTAL_ARRAY_FUNCTION=1

$ pip install https://github.com/Quansight-Labs/uarray/archive/master.zip
