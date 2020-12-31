Follow the steps to get started:
1) Download or Clone this repository on your system.
2) Write "npm install" to command line to install all the required dependencies
3) Write "node index.js" to execute the project


How to use DB

1) Create a instance of DB. 
    const db = new DB();
    
2) Then Create a datastore by using "db.createDatastore(name,path)" method, name is required, path is optional, if not provided it will  create the datastore in the datastore folder.
  
3) Call "db.useDatastore(name,path)" method to use(create,read and delete operations) the datastore.

4) To insert a key-value pair in the datastore use "db.insert(key,value,timeToLive)" method,
    key and value are required,
     timeToLive is optional, if provided then it should be the integer denoting the number of seconds after which we can't read and delete that key from the database
     
5) To get the value associated with a key use "db.get(key)" method in which key is a required field

6) To delete a key use "db.delete(key)" method in which key is a required field
