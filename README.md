# Install

1. Get files from `packages` folder to a Linux device

1. Install `libusb`:
    ```
    cd libusb
    sudo apt install *.deb
    ```

1. Extract archives

    ```
    sudo tar -xvf librealsense.tar --absolute-names
    sudo tar -xvf pylibrealsense.tar --absolute-names
    ```

    or 
    
    ```
    mv librealsense.tar /
    mv pylibrealsense.tar /
    cd /
    sudo tar -xvf librealsense.tar
    sudo tar -xvf pylibrealsense.tar
    ```

# Test

```
python3

from librealsense2 import librealsense2 as rs
list(rs.context().devices)
```
