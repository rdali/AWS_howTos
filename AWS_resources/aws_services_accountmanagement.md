# AWS Services that help with Account Management

I have been delving more and more into AWS for the last few years. I am quite impressed with the number of services and capabilities available for both small and large teams. Here are a list of tools to be aware of if you are managing your team's AWS account(s).

## Monitoring and Governance

#### [AWS cloudtrail](https://aws.amazon.com/cloudtrail/)

AWS cloudtrail logs all events/API calls made within an AWS account. If you want to trace who deleted the S3 buckets or who created a resource, cloudTrail is a good place to start. AWS CloudTrails is enabled by default but history is retained for only 3 months unless you extend it.


#### [AWS Config](https://aws.amazon.com/config/)

AWS Config assesses, audits and records configuration changes over time. If you want to make sure that ssh ports on all your instances are closed or that none of your S3 buckets have public access, for example, AWS Config is a good resource. AWS Config can trigger notifications when resources become non-compliant with the rules you set. Automated [remediation actions](https://docs.aws.amazon.com/config/latest/developerguide/remediation.html) can also be set through [SSM](https://aws.amazon.com/blogs/mt/implement-aws-config-rule-remediation-with-systems-manager-change-manager/).


#### [AWS Trusted Advisor](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)

AWS Trusted Advisor asseses your AWS environemnt and provides recommendations based on best practices. It looks into 5 areas:

- Cost Optimization
- Performance
- Security
- Fault Tolerance
- Service Limits

AWS Trusted Advisor is enabled for all customers for core checks only. All checks are available with Business and Enterprise support plans.


#### [AWS Personal Health Dashboard](https://aws.amazon.com/premiumsupport/technology/aws-health-dashboard/)

While AWS has [Health Dashabords](https://health.aws.amazon.com/health/status) that display the health status of its services across the globe, the Personal Health Dashboard is customized with the services your account uses. It also shows upcoming maintenance events.

#### [AWS tagging](https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html)

AWS allows you to add Key:value tags on most of its resources. Tagging can help you with resource organization, cost allocation, automation and access control.



## Automation and standardization

#### [AWS Systems Manager (SSM)](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html)

AWS Systems Manager (SSM) is a collection of services that help you manage your operations both on AWS and on-premise. It can be thought of as an operation hub. It can automate software installation on your EC2 and manage patching, as well as many other features.  

#### [Cloudfromation](https://aws.amazon.com/cloudformation/) and [Cloud Development Kit (CDK)](https://aws.amazon.com/cdk/)

Infrastructure As Code (IaC) is a best practice that reduces manual labor and errors and makes it easier to reproduce/standardize systems. AWS supports IaC through many different languages, with Cloudfromation and CDK being AWS-native.

Cloudformation is based on yaml or json templates. It is powerful but can be painful to write at times. The AWS Cloud Development Kit (CDK) might be more your style if you prefer to write IaC using a programming language instead (6 currently supported: TypeScript, JavaScript, Python, Java, C#/.Net, and Go).

#### [Service Catalog](https://aws.amazon.com/servicecatalog/)

If you want to curate resources and make templates available to your employees for standardizing tools or to restrict usage to only authorized products, Service Catalog can help! 



## Billing and Budgets


#### [Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)

Cost Explorer allows you to visualize and manage your AWS costs and usage. It also allows you to create reports, forecast future usage and analyze usage across accounts or resources with the help of AWS allocation tags.

#### [Savings Plan](https://aws.amazon.com/savingsplans/)

AWS has a Savings Plan program that gives you access to better pricing than on-demand pricing when you commit to a certain amount of spending. If much of your workload is on AWS, and you will be getting a bill every month, you might as well commit to what your minimum spending is and get a discount!


#### [AWS budgets](https://aws.amazon.com/aws-cost-management/aws-budgets/)

AWS Budgets allow you to set spending limits and create notifications when you are approaching these limits at different thresholds. It is never a good surprise when you forget a costly service on and receive a huge bill. All my AWS accounts have budgets set on them and notifications at 70% thresold.



## Multi-Account Management

It has become more and more common for organizations to have several accounts to separate concerns. There are several AWS Services that help with Account Managment.

#### [AWS organizations](https://aws.amazon.com/organizations/)

AWS Organizations allows you to create a logical grouping of multiple accounts. It helps you centrally manage access policies across accounts,  govern access to AWS services, resources and regions and enables consolidated billing which gives you access to pricing benefits from aggregated usage.


#### [AWS Control Tower](https://aws.amazon.com/controltower/)

AWS Control Tower is AWS Organizations on steroids. AWS Control Tower runs on top of AWS Organizations but adds automation, guardrials and governance.

#### [AWS Resource Access Manager](https://aws.amazon.com/ram/)

AWS Resource Access Manager allows you to securely share AWS resources across multiple accounts. If you want to share a VPC, a transit gateway, or other AWS resources, check out AWS RAM!





