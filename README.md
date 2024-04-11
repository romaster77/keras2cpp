# keras2cpp


colab syntax
based on https://github.com/PaulusCereus/PaulusCereus.git



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