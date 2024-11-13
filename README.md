Convert the code into the python file
Extract the requirements.txt and then make a docker file
In the docker file

---------------------------------------------------------------------------------------------------------
#For Docker code
---------------------------------------------------------------------------------------------------------
FROM python
WORKDIR /app
COPY . /app
RUN pip install --no-cache-dir -r requirements.txt
CMD ["python3","app.py"]
--------------------------------------------------------------------------------------------------------

Write the above code as it is 
Make sure your app.py is the name of the file you want to be using for the project.

And in the requirements.txt you can save the code like the way you want


To make a docker image
Write the following code

TO BUILD THE IMAGE
docker build -f path_to_your_dockerfile -t myfirstpythonappp .

TO DELETE THE IMAGE
docker rmi <image_id_or_name>

