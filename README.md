# dataset for object detection

[Open Images Dataset V6 + Extensions](https://storage.googleapis.com/openimages/web/index.html) - 15,851,536 boxes on 600 categories

    git clone https://github.com/pythonlessons/OIDv4_ToolKit.git
    pip install -r OIDv4_ToolKit/requirements.txt
   
    python main.py downloader --classes 'Vehicle registration plate' 'Traffic sign' 'Traffic light' Car Bus Truck Person --type_csv train --limit 2000
    python main.py downloader --classes 'Vehicle registration plate' 'Traffic sign' 'Traffic light' Car Bus Truck Person --type_csv test --limit 200
    
Result:
* train --limit 10 on Colab
![download_1](download_1.jpg)
* test --limit 2 on Colab
![download_2](download_2.jpg)

 ## Convert annotaion label to XML format
 
    python oid_to_pascal_voc_xml.py
      
 ## Convert XML to YOLO v3 file structure
 
    python [XML_to_YOLOv3.py](https://github.com/pythonlessons/TensorFlow-2.x-YOLOv3/blob/master/tools/XML_to_YOLOv3.py)
