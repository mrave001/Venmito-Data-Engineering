# Venmito Data Engineering Project

Name: Miguel Ravelo

Email: mrave001@gmail.com

GitHub Username: mrave001

## Requirements
The project was be completed using the following:
1. Jupyter Notebook with Python code in .ipynb format
2. Language: Python version 3.8 or higher
3. Python packages: 
    - pandas
    - numpy 
    - matplotlib 
    - yaml 
    - xml.etree.ElementTree 
    - os 
    - plotly.express
4. Visual Studio Code or an IDE (optional)

## File/Folder Structure

- `data`: Contains all the original data files that are parsed in this project to parse
- `README.md`: README file created for the solution to the Venmito Data Engineering Project
- `Data_Storage`: Contains all of the data files persisted by the code in the form of CSV files
- `Venmito_MiguelRavelo.ipynb`: Jupyter Notebook  file containing all of the data parsing code, analysis of the datasets and suggestions

## Solution Description

For my Venmito data engineering project, I have chosen to use Jupyter Notebook to interactively develop my code and to display
data results and visuals of the analysis performed on the various datasets in the provided data folder by Venmito. I chose to
use Jupyter Notebook because not only can I use it to develop Python code, but I can also add markdown notes to help guide the 
user throughout my project. More importantly, Jupyter Notebook allows me to access all of the powerful data manipulation and
visualization libraries for Python, such as Pandas, Numpy and Matplotlib just to name a few. In addition, users that already
have Jupyter Notebook install on their machine, don't need a particular IDE to run the code, they can simply boot up Jupyter
Notebook via the Terminal/CLI from the directory of their choosing and the webserver of Jupyter  Notebook running on localhost
at port 88 shall automatically pop-up and allow the users to access files and notebooks within that same directory.  

As par of my contribution to this project, I created a Jupyter Notebook called `Venmito_MiguelRavelo.ipynb` where all of my 
Python code can be accessed and ran interactively by anyone with the above listed requirements installed. Below I will provide 
clear instructions on how to run the Python code in the notebook but first I shall explain the flow followed in this notebook
and how I used it to address each of the required portions of this project, Data Ingestion, Data Matching and Conforming and 
Data Analysis.

For my design of the `Venmito_MiguelRavelo.ipynb` notebook in this repo, I began with a Python function for each file type that would 
parse each particular file, ingest the contents of those files and then create a Pandas dataframes for each of those data files. 
The reason for creating these Pandas dataframes for each file type is to easily manipulate and reorganize the contents later on, 
as per the Data Matching/Conforming and Analysis requirements of this project. There's a read_json function, a read_yaml function,
a read_xml function. One for each file type that needs to be parsed. Once any of these functions is passed the path in the
data folder where files are located, its respective dataframe is created and the code proceeds with transforming these dataframes
to more commonized format and a suitable form for further analysis. Once all reorganizations and formatting is complete 
(data matching and conforming), including any mergers between dataframes for comprehensive analysis, the Pandas .to_csv() method
is ran on each reorganized dataframe and it is saved in an established file path in a folder called `Data_Storage`.

Then we proceed with code used for the data analysis on that reorganized data for each particular file(s). This is when the code 
will output new tables of with insight information and even plots to visually demostrate further analysis reorganized data. I have
provided all throughout this notebook markdowns that will guide the user and let them know in which section of the code they are 
in and what the purpose of that section is. Finally, the last kind of section that will be found for each analyzed dataframe is the
Suggestion section. These are markdown sections with my personal suggestion to Venmito on actions they can take to improve their 
business based on the previous data analysis. 


## File Instructions
When a user accesses this repository, they will find several files that I have contributed to this repo in addition to what was
previously there. They will find the `Venmito_MiguelRavelo.ipynb` file and the `Data_Storage` folder where .csv file will 
automatically get saved to persist the reorganized and reformatted datasets. As mentioned before, the user doesn't need to use
an IDE to launch and run a Jupyter Notebook. Once Jupyter is installed on the user's machine, they can simply boot up the 
Jupyter webserver that houses the directory of this repo and open up the `Venmito_MiguelRavelo.ipynb` from there. Alternatively,
several editors like Visual Studio Code have extensions that would allow the user to run a Jupyter Notebook from within the 
editor. Once the notebook is opened on the webserver, the user will be presented with an interactive interface with cells containing
the code I have written in Python and markdown notes for guidance. The user can simple run each cell block one by one by first 
selecting the cell block and then pressing the play button in the top menu or the keyboard shortcut: Shit+Enter will run all 
the code in the selected cell. Each cell block of code in this notebook must be ran in sequential order in order to provide the
expected output. If needed users can restart and clear all outputs in the notebook by clicking the Kernel-> Restart & Clear Output
in the top menu of the notebook. This can prove to be useful when needing to rerun a previously ran cell or section of code.
