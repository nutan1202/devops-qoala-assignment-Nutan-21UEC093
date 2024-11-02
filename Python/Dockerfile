FROM python:3.9
#correction of spellings of app 
WORKDIR /app  
#correction of spellings of app 
COPY app.py /app  

# For package installations
RUN pip install flask netifaces 
#correction for syntax for writing the port number
EXPOSE 8000  

CMD ["python", "app.py"]  
