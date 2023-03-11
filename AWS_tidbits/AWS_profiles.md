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


# Do you have multiple accounts and are starting to use the CLI?

Use AWS named profiles for the AWS CLI to interact with different accounts.

<details>
    <summary>
    	**Using named profiles** (click me)
    </summary>
    <p>
    To set up a new profile:  
		`aws configure --profile myprodprofile`   
	 To use a specific profile:  
		`aws s3 ls s3://mybucket --profile myprodprofile`    
	
[Reference](https://docs.aws.amazon.com/toolkit-for-visual-studio/latest/user-guide/keys-profiles-credentials.html) 
	
   </p>
</details>


Now you can store credentials from many accounts and use them in the same session!


[Reference](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html)


# Now You Know!