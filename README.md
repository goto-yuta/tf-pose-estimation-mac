# About this repository
Cloned repository of [this](https://www.github.com/ildoonet/tf-openpose) which has already deleted.  
Some scripts are changed in order to use in MACOS.  

# Usage
## Preparation
Before cloning this repository, run the commands below.  
```
git clone https://github.com/cocodataset/cocoapi.git
cd cocoapi/PythonAPI
python setup.py build_ext install
```

Next, clone this repository and run the command below after cloning this repository.  
```
pip install -r requirements.txt
cd tf_pose\pafprocess
swig -python -c++ pafprocess.i
python setup.py build_ext --inplace
cd ../../
python setup.py install
```

At this point, you are in ready state.  

## How to Run
Run the code below.
```python
python run.py --model=cmu --image=path_to_image
```
