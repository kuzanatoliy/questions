# Identity and Access Management (IAM)

<details>
  <summary>What is an IAM?</summary>

AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources. With IAM, you can centrally manage permissions that control which AWS resources users can access. You use IAM to control who is authenticated (signed in) and authorized (has permissions) to use resources.

[More >>](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)

</details>

<details>
  <summary>What are IAM users?</summary>

The "identity" aspect of AWS Identity and Access Management (IAM) helps you with the question "Who is that user?", often referred to as authentication. IAM users are not separate accounts; they are users within your account. Each user can have its own password for access to the AWS Management Console. You can also create an individual access key for each user so that the user can make programmatic requests to work with resources in your account.

[More >>](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction_identity-management.html)

</details>

<details>
  <summary>What is a connection between policies and users or groups?</summary>

IAM users are identities in the service. When you create an IAM user, they can't access anything in your account until you give them permission. You give permissions to a user by creating an identity-based policy, which is a policy that is attached to the user or a group to which the user belongs.

[More >>](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction_access-management.html)

</details>
