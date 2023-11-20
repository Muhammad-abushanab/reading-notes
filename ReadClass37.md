# Amazon S3

Amazon Simple Storage Service (Amazon S3) is a scalable object storage service provided by Amazon Web Services (AWS). It allows users to store and retrieve data over the internet, offering high durability, availability, and scalability.

## Features of Amazon S3

1. **Scalability**: S3 can store an unlimited amount of data and handle a virtually unlimited number of concurrent requests, making it suitable for various storage needs.
   
2. **Durability and Availability**: S3 stores data redundantly across multiple locations, ensuring high durability (99.999999999% reliability) and availability.

3. **Security and Access Control**: S3 offers robust security features, including encryption, access control lists (ACLs), and bucket policies, allowing fine-grained control over who can access the stored data.

## Object Key

In Amazon S3, an object key is a unique identifier for an object stored in a bucket. It is similar to a file path in a file system and consists of the object's name and its location within the bucket's namespace. For example, in the key "folder/document.txt":
- "folder/" is the prefix or directory name.
- "document.txt" is the object name.


### Dependencies for Amplify AWS S3 in Android Application

To use Amplify AWS S3 in an Android application, you'll need to include the necessary dependencies in your project:

1. **Amplify Framework**: Include the Amplify Framework library in your project.
2. **Amplify AWS Storage Plugin**: This plugin allows interaction with AWS S3. Include it in your project's dependencies.

Add the following dependencies to your `build.gradle` file:

```groovy
dependencies {
    implementation 'com.amplifyframework:core:1.0.0'
    implementation 'com.amplifyframework:aws-storage-s3:1.0.0'
    // Other dependencies for your Android project
}
```
### Uploading Data to Your Bucket
To upload data to your Amazon S3 bucket using AWS Amplify, you'll need:

- Initialization: Configure and initialize Amplify in your application. This involves setting up necessary plugins for categories like authentication and storage.

- Access Credentials: Ensure your application has the necessary AWS credentials and permissions to interact with the specified S3 bucket. These credentials are typically obtained through AWS Identity and Access Management (IAM) and should have the appropriate permissions to upload objects to the bucket.

- Using Amplify Storage Category: Utilize the Amplify Storage category's methods (e.g., put, uploadFile, etc.) to upload data (files, objects) to your S3 bucket. These methods allow you to specify the bucket, file paths, and additional configurations like ACLs or content types.

### Initializing Amplify Auth and Storage Categories
To initialize the Amplify Auth and Storage categories:

- Amplify Configuration: Configure Amplify with the necessary plugins and categories in your application. Use the Amplify.addPlugin() method to add plugins for the required categories.

- Initialization: After adding the plugins, call the Amplify.configure() method to initialize Amplify, which initializes the configured categories like Auth and Storage.

```java
import com.amplifyframework.Amplify;
import com.amplifyframework.auth.AuthCategory;
import com.amplifyframework.storage.StorageCategory;
AuthCategory authCategory = Amplify.Auth;
Amplify.addPlugin(new AWSCognitoAuthPlugin()); 
Amplify.configure(getApplicationContext()); 
StorageCategory storageCategory = Amplify.Storage;
Amplify.addPlugin(new AWSS3StoragePlugin());
Amplify.configure(getApplicationContext());
```