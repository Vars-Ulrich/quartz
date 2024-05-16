---
sticker: vault//Media/icons/aws-icons/IdentityAndAccessManagement.svg
aliases:
  - IAM
---

# Identity and Access Management

- Global in scale

- Policies written as JSON docs
	- JSON policy doc includes these elements:
		- optional policy-wide information at the top of the doc
		- One or more individual statements
- Two mandatory elements
	- Effect
		- "Allow" or "Deny"
	- Action
		- List of actions that the policy allows/denies
- Four Optional elements
	- Statement ID (Sid)
		- Include an optional statement ID to differentiate between your statements.
	- Principal
		- required only in some circumstances
		- If you create a resource-based policy, you must indicate the account, user, role, or federated user to which you would like to allow or deny access. If you are creating an IAM permissions policy to attach to a user or role, you cannot include this element. The principal is implied as that user or role.
	- Resource
		- If you create an IAM permissions policy, you must specify a list of resources to which the actions apply. If you create a resource-based policy, this element is optional. If you do not include this element, then the resource to which the action applies is the resource to which the policy is attached.
	- Condition
		- Specify circumstances under which policy grants permission

# IAM credentials report
You can generate and download a credential report that lists all users in your account and the status of their various credentials, including passwords, access keys, and MFA devices. It is not used to review permissions granted to a user.

# IAM access advisor
Access advisor shows the service permissions granted to a user and when those services were last accessed. You can use this information to revise your policies. To summarize, you can identify unnecessary permissions so that you can revise your IAM policies accordingly.


[[SAA Course Slides.pdf#page=25&selection=0,0,0,1|SAA Course Slides, page 25]]
