# project-OBJECT DETECTION MODEL
In the following project I have created an object detection model (for detecting the cylinders)

 To make this I have taken refrence form tfod 2.0 odm site & stacksoverflow

    Pretrained model used: ssdd resnet101 v1 fpn 640x640
    
    changes that I made in pipeline.config file:
                    1: no_of_classes = 1
                    2: batch_size = 10
                    3: step_size = 2000
                    4: use_bfloat16: false
                    5: fine_tune_checkpoint type = "detection"
                    6: paths were updated for tf.record file
                    7: I have used tensorflow version 2.8 in this project

 changes to make before running the model:
                 1: upload training_demo.zip file in /content file (then it will automatically get unzip after you run the code)
                 2: unable gpu before starting the runtime
                 3: Incase if you want to improve the accuracy, just open the pipeline.config in training_demo/models/ssd_resnet101_v1_fpn and change line 152 and 162 to 2500 or more

 NOTE: trained model will be stored in /training_demo/exported-models
 
                    
    
 
