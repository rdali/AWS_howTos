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


# Having a hard time remembering your AWS 12 Digit account ID?

You can create an account Alias that would be a lot easier to remember!

 
<details>
    <summary>
    	**Via the CLI** (click me)
    </summary>
    <p>
    To create a new alias:  
		`aws iam create-account-alias --account-alias mynewalias`   
	 To list account aliases:  
		`aws iam list-account-aliases`    
	To delete account aliases:   
	`aws iam delete-account-alias`   
	[Reference](https://docs.aws.amazon.com/cli/latest/reference/iam/index.html#cli-aws-iam)
    </p>
</details>

<details>
    <summary>
        **AWS Console** (click me)
    </summary>
    <p>
1- Sign in to the AWS Management Console.  
2- Open the [IAM console](https://console.aws.amazon.com/iam/).  
3- In the navigation pane, choose Dashboard.     
4- In the right-hand pane under AWS account, choose Customize. If an alias already exists, then choose Edit.  
5- Save changes.   
    </p>
</details>


Now you can use your Alias to sign into your account and can forget the 12 Digit ID!


[Reference](https://docs.aws.amazon.com/accounts/latest/reference/manage-acct-alias.html)


# Now You Know!