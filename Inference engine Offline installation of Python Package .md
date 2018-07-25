**Inference engine install Python Package**
=============

The Inference engine is a Python runtime program that runs on Docker on a foggy device, so it is sometimes necessary to update the relevant suites that Python needs.

**Update the Python Package via the Internet (example below is the installation of the xgboost Package)**
-------------
1. Enter the container running Docker and execute pip install

    ```pip install xgboost```
    
    ![image](https://github.com/minikai/inference_engine_annotation_mqtt/blob/master/pip%20install%20xgboost.png?raw=true)
    
    
**Update the Python Package via the whl file in a no-network environment (example below is the installation of the xgboost Package)**
-------------
1. Put the xgboost package whl file in the c:\inference_engine directory

    ![image](https://github.com/minikai/AFS_Inference_engine_doc/blob/master/whl%E8%B7%AF%E5%BE%91.png?raw=true)

2. Go to the /inference_engine folder in the container that Docker runs.

   ```cd /inference_engine/```
 
3. Use pip install to install xgboost's whl file

   ```pip install xgboost-0.72.1-py2.py3-none-manylinux1_x86_64.whl```
   
     ![image](https://github.com/minikai/inference_engine_annotation_mqtt/blob/master/pip%20install%20whl.png?raw=true)
