# MongoDB Atlas & pymongo Sample Project

This repository contains a very basic example application 
built with the [pymongo](https://docs.mongodb.com/drivers/pymongo)
MongoDB Driver that connects to [MongoDB 
Atlas](https://www.mongodb.com/cloud/atlas). You can use this application
as a starting point and reference when building your Python applications.

## Prerequisites

To build and run this project, you will need:

- Python 3.7 or higher
- The `pymongo` module
- The `dnspython` module
- An Atlas account

## Getting Started

The following instructions explain how to get this project
connected to your instance of MongoDB Atlas.

### 1. Download the Repository

To get started with this sample project, download this repository to your
programming environment. You can clone this project using Git
version control:

```
git clone git@github.com:mongodb-university/atlas_starter_python.git
```

Or you can download the ZIP archive using your browser. If you download
this project as a ZIP archive, 
[unzip the archive](https://www.wikihow.com/Unzip-a-File) before proceeding.

### 2. Install the modules

You can use `pip` to install the necessary Python modules.

```
pip install pymongo dnspython
```

### 3. Configure your Atlas Credentials

1. Open the  `atlas-starter.py` file.

2. On line 8, replace the placeholder text with the connection string 
   to your Atlas cluster. For more information on finding your connection 
   string, see [the Atlas documentation](https://docs.atlas.mongodb.com/driver-connection/).

```python
    client = pymongo.MongoClient(
      "mongodb+srv://<username>:<password>@<cluster-name>/test?retryWrites=true&w=majority")
```

### 4. Run the program

1. At your command prompt, navigate to the `atlas_starter_python` directory.

2. Run the program:

```
python atlas-starter.py
```

Assuming you have the correct connection string, you'll see the program
output. Have fun modifying the code to experiment with pymongo and MongoDB.

## Troubleshooting

Are you having trouble getting connected to your MongoDB Atlas instance?
Double-check the following:

1. Have you replaced the placeholder text with a valid connection string
   provided by the Atlas UI? Read more [here](https://docs.atlas.mongodb.com/driver-connection/)
   for further context.

2. Have you [whitelisted your current IP address](https://docs.atlas.mongodb.com/security-whitelist/)
   in the Atlas UI?
