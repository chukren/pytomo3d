# Installing python dependencies

Pytomo3d has dependancies on the following packages:
1. [obspy](https://github.com/obspy/obspy)
2. [pyflex *devel* branch](https://github.com/wjlei1990/pyflex)
3. [pyadjoint *dev* branch](https://github.com/chukren/pyadjoint)

---

### Manual installation

Wenjie: If you are new to python, [anaconda](https://www.continuum.io/downloads) is recommmended. Please download the newest version(>= Anaconda2-2.5.0) since it already contains a lot of useful python packages, like pip, numpy and scipy.  Old versions is not recommended since it usually embed compliers inside, like gfortran and gcc. It is always better to use comiplers coming from your system rather than the very old ones embeded in anaconda. If you are expert in python, please choose the way you like.

1. downwnload Anaconda for Python 2.7 and 64 bit Linux and install it (http://continuum.io/downloads)(**optional**)

2. install obspy using anaconda.
```
conda install -c obspy obspy
```

Or install from source code:
```
git clone https://github.com/obspy/obspy.git
cd obspy
pip install -v -e .
cd ..
```

3. install pyflex.
```
git clone --branch devel https://github.com/wjlei1990/pyflex 
cd pyflex
pip install -v -e .
cd ..
```

4. Install pyadjoint
```
git clone --branch dev https://github.com/chukren/pyadjoint 
cd pyadjoint
pip install -v -e .
cd ..
```

### Script installation

Wenjie: recommended for experienced user

```
pip install -r requirements.txt
```

---

### Notes
1. If you already have some of the packages, please make sure to update them(not including anaconda)