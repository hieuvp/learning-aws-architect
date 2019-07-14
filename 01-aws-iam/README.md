# AWS Identity and Access Management (IAM)

> Pronounce "**I am**".

## Table of Contents
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [CIA Triad](#cia-triad)
- [Principals](#principals)
  - [Users](#users)
  - [Groups](#groups)
  - [Roles](#roles)
- [Policies](#policies)
  - [Policy Types](#policy-types)
  - [Denying Access with User Policies](#denying-access-with-user-policies)
  - [Denying Access with Group Policies](#denying-access-with-group-policies)
- [Identity Providers](#identity-providers)
- [References](#references)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## CIA Triad

<div align="center"><img src="assets/confidentiality.png" width="600"></div>
<br />

<div align="center"><img src="assets/integrity.png" width="600"></div>
<br />

<div align="center"><img src="assets/availability.png" width="600"></div>

## Principals

### Users

Create users if you want to grant other users access to your AWS account without sharing your login credentials.

### Groups

Groups make it easy to manage access for multiple users.

### Roles

Roles are similar to users as they hold an AWS identity with permissions.
Roles are often used if you e.g. want to grant access to AWS resources that the user normally does not have.

Another scenario would be that you want to grant an application access to your AWS resources without exposing your AWS credentials.

## Policies

With policies you can define permissions for users, groups and roles.
Policies are the building blocks to define what action can be performed for what resource.

<div align="center"><img src="assets/permission-statement.png" width="600"></div>

### Policy Types

<div align="center"><img src="assets/policy-types.png" width="900"></div>
<br />

**`Managed Policies`** - Standalone identity-based policies that you can attach to multiple users, groups, and roles.

- **`AWS Managed Policies`**: Managed policies that are created and managed by AWS.
	
- **`Customer Managed Policies`**: Managed policies that you create and manage. Customer managed policies provide more precise control over your policies than AWS managed policies.

**`Inline Policies`** - Policies that you create and manage and that are embedded directly into a single user, group, or role.

### Denying Access with User Policies

### Denying Access with Group Policies

## Identity Providers

Identity providers enable you to let users gain access to your AWS resources with the help of an external identity provider (IdP).

<div align="center"><img src="assets/identity-providers.png" width="900"></div>

## References

- [AWS fundamentals: What is IAM?](https://medium.com/@pmuens/aws-fundamentals-what-is-iam-b57f2fb88f66)
