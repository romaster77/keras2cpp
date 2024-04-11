# keras2cpp
generate cpp from python

colab syntax

based on repo https://github.com/PaulusCereus/PaulusCereus.git

## result
```
build/example.model
build/keras2cpp
```


## run
```
# ----------------------------------
import os

# ----------------------------------
# upload folder to colab
! git clone https://github.com/romaster77/keras2cpp.git

# ----------------------------------
# change dir
os.chdir('keras2cpp')
!mkdir build 
os.chdir('build')


# ----------------------------------
# generate example.model
!python3 ../python_model.py 

# ----------------------------------
# generate keras2cpp (build cpp)
! cmake ..
! cmake --build .

# ----------------------------------
# test result
! ./keras2cpp

```
