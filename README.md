# SFR-Cheques-Draft
I am making a model for SFR using the cheques dataset which can read the Name, date, sign, account number, amount in words line 1 and 2,  amount in number, m number and the in favor name separately and print the output for each cheque separately.

# data.yaml file
In this we have to add a data.yaml file to the data stored in yolov9 directory
train: /content/yolov9/data/train/images  
val: /content/yolov9/data/val/images      
test: /content/yolov9/data/test/images 
nc: 9
nc: 9
names: ['Accnt Number', 'Amnt in No.', 'Amnt in Wrds Line 1', 'Amnt in Wrds Line 2', 'Date', 'In Favor Name', 'M Number', 'Name', 'Sign' ]

# plots.py
In plots.py line 86 instead of 'getsize' we will be using 'getbbox' 
w, h = self.font.getbbox(label)[2:] 


