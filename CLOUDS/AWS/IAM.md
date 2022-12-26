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

<details>
  <summary>What is an Attribute-based access control (ABAC)?</summary>

Attribute-based access control (ABAC) is an authorization strategy that defines permissions based on attributes. In AWS, these attributes are called tags. You can attach tags to IAM resources, including IAM entities (users or roles) and to AWS resources. You can create a single ABAC policy or small set of policies for your IAM principals. These ABAC policies can be designed to allow operations when the principal's tag matches the resource tag. ABAC is helpful in environments that are growing rapidly and helps with situations where policy management becomes cumbersome.

</details>

<details>
  <summary>What is a role-based access control (RBAC)?</summary>

The traditional authorization model used in IAM is called role-based access control (RBAC). RBAC defines permissions based on a person's job function, known outside of AWS as a role. Within AWS a role usually refers to an IAM role, which is an identity in IAM that you can assume.

</details>

<details>
  <summary>What are IAM roles?</summary>

IAM roles are a secure way to grant permissions to entities you trust. Roles are an IAM identity that you can create in your account that has specific permissions. An IAM role has some similarities to an IAM user. Roles and users are both AWS identities with permissions policies that determine what the identity can and cannot do in AWS. However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone who needs it.

[More >>](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html)

</details>

<details>
  <summary>What types of policies could be attached to role?</summary>

**Trust policy** – Policy which defines which identities can assume the role. Creating a role with the IAM console automatically creates a default trust policy that you can customize. A role can have only one trust policy.

**Permissions policy** – Policy which defines which AWS resources a role can access and the actions it can perform on those resources. Permissions policies can be AWS managed policies, customer managed policies, or inline policies attached directly to the role. You can attach multiple permissions policies to an IAM role.

</details>
