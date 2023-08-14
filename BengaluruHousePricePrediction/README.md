This data science project series walks through step by step process of how to build a real estate price prediction website. We will first build a model using sklearn and linear regression using banglore home prices dataset from kaggle.com. Second step would be to write a python flask server that uses the saved model to serve http requests. Third component is the website built in html, css and javascript that allows user to enter home square ft area, bedrooms etc and it will call python flask server to retrieve the predicted price. During model building we will cover almost all data science concepts such as data load and cleaning, outlier detection and removal, feature engineering, dimensionality reduction, gridsearchcv for hyperparameter tunning, k fold cross validation etc. Technology and tools wise this project covers,

1. Python
2. Numpy and Pandas for data cleaning
3. Matplotlib for data visualization
4. Sklearn for model building
5. Jupyter notebook, visual studio code and pycharm as IDE
6. Python flask for http server
7. HTML/CSS/Javascript for UI

# Demo Video of the Project 
<br>
![***demo***](https://github.com/dattabiplab/DataScience-Projects/blob/509dee4101673d496a1361bdb03181253aa3b4b7/BengaluruHousePricePrediction/bhp_demo.mp4)
# Deploy this app Locally

1. Download the BengaluruHousePricePrediction project folder in a respective drive or folder.
2. Download ***nginx***.
3. Copy the downloaded nginx folder to "Drive C" ***Program Files*** folder.
4. Copy the path location of "client" folder present in the project folder.
5. Open the ***nginx.conf*** file in conf folder of the nginx folder.
6. Paste this code at the respective position from the
   ![nginx-fix](https://github.com/dattabiplab/DataScience-Projects/blob/509dee4101673d496a1361bdb03181253aa3b4b7/BengaluruHousePricePrediction/nginx-fix.png) photo.
   ```
 	location / {
            root   "C:\Users\BIPLAB DATTA\BHP\client";
            index  index.html index.htm app.html;
        }
   ```
8. In *root* paste the path of the **client** folder and Save the file.
9. Open the terminal(such as Git Bash) in "server" folder of the project.
10. Type ```python server.py``` and start the server.
11. Now go to the "nginx" folder of the Program Files and double-click on the ***nginx.exe*** app and Start the app.
12. Open the browser and type ```localhost``` and the app will be running there.
