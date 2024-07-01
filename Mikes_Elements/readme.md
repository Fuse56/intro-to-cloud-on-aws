### Fieldbooks.Admin Security Policy

- The file in this directory called `"Fieldbooks_Admin_Sec_Policy.json"`
  is a **_working_** policy that effectively allows CRUD access to the three S3 buckets that contain the Field books files.

- All other buckets can be _listed_ but their contents cannot be viewed or acted upon.

- Within the Security Policy, the `"ListAllBucketsRequired"` Sid is a a mandatory element in order for the user to utilize the `"CrudAccess"` Sid.
- For unknown reasons, you can't add specific resources to the `ListAllMyBuckets` Action. You must use an asterisk that allows listing of all buckets.
