# Natural Language Processing for the Wellington Residents Survey 

The purpose of this project is to analyse unused text data from the Wellington Residence survey. Currently the only data from the survey used is numerical. The purpose of this piece of work is to identify the top things that people are answering in the text answers. 

The project is to apply natural language processing to free form text.
The model developed is a top2Vec model. This allows the program to identify different topics throughout all the responses and identify what each topic represents. 

To help deliver this project to the users a FastAPI has been developed. This is a hosted web server that allows the user to upload a text file and get real time results from the model.

Users need to upload a text file where each comment is in a different line. The program can handle it as a csv file. The data is then pre-processed before a model is applied to it. This includes removing newline characters and stop words. The stop words have been identified using an open library of English stop words.

For testing you can read in your own file. And then test all the models on it. Or you can just run all the functions before the fastapi section. 
Currently the functions and the fastapi are in the same Jupyter notebook but this will get split out to be two different notebooks. A main and a model functions. 
