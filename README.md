**Serialization and Deserialization in Java**

Introduction
Serialization and deserialization in Java are processes used to convert an object into a byte stream and then reconstruct the object from that byte stream. This is commonly used for saving an object's state to a file, sending an object over a network,
or caching objects.


Serialization - Serialization is the process of converting an object into a byte stream. This byte stream can be saved to a file, sent over a network, or stored in memory.This is done using the “java.io.Serializable” interface.

Deserialization- Deserialization is the process of reconstructing an object from a byte stream.This is done using the “ObjectInputStream “class.


**Advantages of Serialization and Deserialization in Java**


1. Persistence
Storing Object State: You can store the state of an object to a file or a database, allowing you to save and retrieve objects across different sessions or runs of a program.
2. Transmission
Network Communication: Objects can be serialized and sent over a network, making it easier to transfer complex data structures between different parts of a distributed system or different applications.
3. Deep Copying
Cloning Objects: Serialization can be used to create a deep copy of an object. By serializing an object and then deserializing it, you get a new object with the same state as the original.
4. Flexibility
Custom Serialization: You can customize the serialization process for special needs (e.g., handling non-serializable attributes, compressing data).
5. Platform Independence
Cross-Platform: Serialized Java objects can be moved across different platforms (Windows, Linux, etc.), retaining their state without compatibility issues.


**Process of Serialization and Deserialization**
Serialization

Marking classes as serializable - A class must implement the java.io.Serializable interface 

ObjectOutputStream - This class is used to write objects to an output stream.

Writing objects to a stream - When an object is passed to the writeObject() method of ObjectOutputStream



Deserialization 

Creating an Input stream - The ObjectInputStream class is used to read objects from an input stream. 

Reading objects from a stream - When an object is read using the readObject() method of ObjectInputStream

Example code

Student.java
![Screenshot from 2024-07-19 08-52-39](https://github.com/user-attachments/assets/15a326de-a7b7-41db-9910-ed485f36e07a)



Main.java
![Screenshot from 2024-07-19 08-52-31](https://github.com/user-attachments/assets/32f89f06-0523-4217-8529-f7efaeecb2f9)
















