# S3 Bucket with Options for Access Control, Encryption, and Versioning

This CloudFormation template creates a basic S3 bucket for object storage in AWS. It provides options to customize access control, encryption, and object versioning through user-defined parameters.

**Key Features:**

* S3 Canned ACLs:
    Choose from pre-defined access control lists (e.g., PublicRead, Private) to simplify permission management for your bucket.
* Default Server-Side Encryption:
    Enable encryption for objects at rest with the option to use a custom AWS Key Management Service (KMS) key.
* Object Versioning: Configure versioning for your bucket to maintain a history of object changes.

  **Parameters:**

* S3 Bucket Name:
    Specify the desired name for your S3 bucket (3-63 characters, letters or numbers, must start and end with a letter or number).
* Bucket Access Control List (ACL):
    Select a canned ACL to define access permissions for the bucket. Defaults to "None" (no canned ACL applied).
* Enable Default Encryption: Choose "true" to encrypt objects by default, or "false" to disable encryption. Defaults to "true".
* KMS Key Id (Optional):
    Provide a valid KMS Key ID to use for custom encryption. Defaults to a placeholder value.
* Object Versioning:
    Set to "Enabled" to enable versioning, or "Suspended" to disable it. Defaults to "Suspended".

**Outputs:**

* Bucket URL:
    The public URL for accessing your S3 bucket (e.g., [invalid URL removed]).
* Bucket ARN:
    The Amazon Resource Name (ARN) uniquely identifying your S3 bucket.

**Benefits of using this template:**

* Simplified S3 Bucket Creation:
    Easily configure basic S3 bucket features through user-friendly parameters.
* Security Enhancements:
    Enforce access control and optional encryption for improved data security.
* Versioning Option:
    Maintain historical versions of your objects for potential rollback or audit purposes.

<p align="center"><b><big>Getting Started</big></b></p>

Replace the placeholder values for KmsKeyId with a valid KMS Key ID if you intend to use custom encryption.
Deploy this template in your AWS CloudFormation stack.
Access the Outputs section to retrieve the Bucket URL and Bucket ARN for further use.
