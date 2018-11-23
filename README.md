# CloudFormation-Workshop-201811

## Exercise 1a
Basic EC2 Template

## Exercise 2a
EC2 Instance with AMI Mapping

## Exercise 2b
EC2 Instance with Dynamic Parameters

## Excercise 3a
Creating a Conditional EC2 Instance

## Exercise 3b
Adding resources to an existing stack
NOTE: This stack is will fail to create successfully. This is by design to demonstrate an 'UPDATE_ROLLBACK_FAILED' state.

To simulate an 'UPDATE_ROLLBACK_FAILED' state, perform the following:

* Launch template 3a in eu-west-1
* Perform and Out-of-Band change in the CloudFormation Console:
    1. Update in the instance created in 3a and associated it with a different security group
    2. Delete the security group created in 3a
    3. Update the stack created in 3a with this stack (3b)

## Exercise 3c
Correcting the previous stack - update the stack with this stack instead after performing a 'Continue Update Rollback'