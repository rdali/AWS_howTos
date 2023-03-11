<style>
details > summary {
  padding: 12px 12px;
  background-color: #f0f8ff;
  border: none;
  box-shadow: 1px 1px 1px grey;
}

details > p {
  border-radius: 0 0 0px 0px;
  background-color: #f0f8f7;
  padding: 10px 15px;
  margin: 0;
  border-left-width: 5px;
  border-left-style: solid;
  border-left-color: #b3dbff;
  border-radius: 0px;
  }
</style>


<img src="vecteezy_did-you-know-sticker-vector_7688896.jpg"  width="30%" height="30%">


# Do you have several AWS credentials and are confused which one is being used?

AWS has a defined Default Credential Provider Chain which dictates the order of which credentials it uses in the case where there are several.
 

The Default Credential Provider Chain Order for Java SDK is:

1- Environment variables: "**AWS\_ACCESS\_KEY\_ID**" and "**AWS\_SECRET\_ACCESS\_KEY**".   

2- Java system properties: **aws.accessKeyId** and **aws.secretAccessKey**. 

3- Web Identity Token credentials from the environment or container.

4- The default credential profiles file: typically located at ~/.aws/credentials

5- Amazon ECS container credentials: loaded from the Amazon ECS if the environment variable AWS\_\CONTAINER\_CREDENTIALS\_RELATIVE\_URI is set.  

6- Instance profile credentials: used on EC2 instances, and delivered through the Amazon EC2 metadata service.


[Reference](https://docs.aws.amazon.com/sdk-for-java/v1/developer-guide/credentials.html)


# Now You Know!