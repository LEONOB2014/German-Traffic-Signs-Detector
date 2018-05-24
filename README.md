# Deep Learning Challenge Kiwi-Campus Solution
## Andres Leonardo Becerra L.

This repository contains the 3 solution model to the Challenge to perform classification of German Traffic Sign dataset http://benchmark.ini.rub.de/Dataset_GTSDB/ and includes:

1. Create a *GitHub* ([https://github.com/](https://github.com/)) repository and name it "German Traffic Signs Detector".
2. Create an [app.py](http://application.py) file, which will store a *Click* application ([http://click.pocoo.org/5/](http://click.pocoo.org/5/)); this will be the main program, and you will implement several comands ([http://click.pocoo.org/5/commands/](http://click.pocoo.org/5/commands/)), which are related to the rest of the tasks of this challenge. 
3. Create directories with the following structure:
```
      German Traffic Signs Detector
        |
        |-images/
                |-train/
                |-test/
                |-user/
        |-reports/
                |-model1.ipynb
                |-model2.ipynb
                .
                .
                .
        |-models/
                |-model1/
                    |-README.md
                    |-saved/
                |-model2/
                    |-README.md
                    |-saved/
                .
                .
                .
        |-README.md
            |-requirements.txt
        |-app.py
```
The requirements are included in `requirements.txt` file
**Task 2 (15 points)** 

Create a *download* command that will download all data from the *German Traffic Signs Dataset* ([http://benchmark.ini.rub.de/?section=gtsdb&subsection=dataset](http://benchmark.ini.rub.de/?section=gtsdb&subsection=dataset)). This will store the the data set inside an *images* folder.

The train folder contains images for training the models; the test folder  have images on which you will validate your models; and finally, the user folder is left empty, we will put our own images there to make our own tests on your code. 

From the total of the images in the data set, 80% are left for training and 20% for testings the models.

The program is executed as follows:

    python app.py download

**Task 3 (15 points)**  

Create, train and save a logistic regression model using scikit-learn ([http://scikit-learn.org/stable/](http://scikit-learn.org/stable/)). 

**Task 4 (20 points)**

Create, train and save a logistic regression (or softmax) model using TensorFlow ([https://www.tensorflow.org/](https://www.tensorflow.org/))

**Task 5 (35 points)**

Create, train and save a LeNet model ([http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf](http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf)) in Tensorflow. 

**Task 6 (10 points)**

Create an application that will use a chosen model and run inference on images saved in a particular directory. For each image in such directory you should show a window with the image together with its label. It should be executed as follows:

    python app.py infer -m [chosen model] -d [directory with user data]

**Further notes:**

Task 3,4,5 are executed as follows:

    python app.py train -m [chosen model] -d [directory with trainig data]

    python app.py test -m [chosen model] -d [directory with test data]

Each of the previous two commands generate as output the accuracy of the selected model.

Each model implemented (tasks 3, 4 and 5) includes a description of the model in a [READM](http://readm.md)[E[.md](http://readm.md) inside that model's directory. Also, there is a report for each of the models, which is saved from models/model1/saved/ 




