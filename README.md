# mongowrapper
Mongo DB light weight wrapper class
This class performs the basic CRUD operation on Mongo database for .net application
This class is written in .net standard and is compatible with .net framework and .net core

Pre-requisites:
You need an entity class which will be used for CRUD operation on Mongo. This entity class should inherit the MongoEntity base class.

Example of the entity class:

    public class Person : MongoEntity
    {
        public override string _id { get; set; }

        public string Name { get; set; }

        public string Address { get; set; }

        public string City { get; set; }

        public Person()
        {
            _id = Guid.NewGuid().ToString();
        }
    }
    
Look into the Test cases for the usage
      
      
