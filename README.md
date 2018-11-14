# How Serious is your Hepatitis

**Prerequisites**

1) You need to have Tableau Desktop
2) You need to have installed Tabpy
        - Use this command *pip install tabpy-server* in the command prompt to install the Tabpy
        - Once this isntalled, look out for the location where it got installed in the cmd prompt. The location may look like this
                    \python\python36-32\lib\site-packages\tabpy_server
        - Once you are in the above location, you can look for the file called *startup.sh*. 
        - Now start the conda environment and run *sh startup.sh*
        - This will create a local server and you can verify the Tableau name when you launch *http://localhost:9004/*


**FILES TO CONSIDER:**

1) *Random Forest.ipynb* (Jupyter Notebook)
2) *Heapatitis Detector.twbx* (Tableau Dashboard)
3) *https://www.openml.org/d/269* (Download the dataset and store it as *hepatitis.csv*)

**STEPS**

1) Make sure you started the Tabpy server ( you can refer to the last steps of Prerequisites)
2) Now that the tableu server is started, you can run the jupyter notebook
3) After you run the jupyter notebook, you can look for this URL *http://localhost:9004/endpoints* to look for *predictHepatits* method we deployed using the python code in jupyter notebook
4) Now, open the Tableau workbook *Heapatitis Detector.twbx* and make sure you navigate to 

        Help -->  Setting and Performance ---> Manage External Service Conenction
        
5) Type in the server as *localhost* and and port as *9004* and thats it, the Tabpy is configured and you should able to run the viz


