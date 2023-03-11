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

# AWS account best practices

This is a living document that will keep growing to highlight AWS Best Practices!


<details>
    <summary>
        **Create an admin user and avoid using the root account** (click me)
    </summary>
    <p>
    
  The root user has full priviledges to the AWS account. For security purposes, it is 		recommended to limit the use of the root account. For daily processes, you can set up an [administraor account](https://docs.aws.amazon.com/singlesignon/latest/userguide/get-started-assign-account-access-admin-user.html).
    
   [Reference](https://docs.aws.amazon.com/accounts/latest/reference/best-practices-root-user.html)
   </p>
</details>


<details>
    <summary>
        **Enable MFA on user sign-ins, especially for the root user** (click me)
    </summary>
    <p>
    
  Multi-factor Authentication (MFA) allows you to secure your accounts and reduces the risk of being hacked.
    
  [Reference](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable.html)
    </p>
</details>


<details>
    <summary>
        **Grant Least Privilege Access Required** (click me)
    </summary>
    <p>
     For better security, set up your IAM policies to allow only the required tasks.
     
   [Reference](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege)
    </p>
</details>

<details>
    <summary>
        **Set Up AWS budgets and account monitoring** (click me)
    </summary>
    <p>
    To avoid unexpected bills, add budgets and notifications on each account.
          
   [Reference](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-best-practices.html)
    </p>
</details>

<br/>
