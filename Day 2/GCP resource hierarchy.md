# GCP resource hierarchy

## GCP projects

* All the resources you use, whether they're virtual machines, cloud storage buckets, tables and big query or anything else in GCP are organized into projects. Optionally, these projects may be organized into folders. Folders can contain other folders. All the folders and projects used by your organization can be brought together under an organization node. Projects, folders and organization nodes are all places where the policies can be defined

* Projects are the basis for enabling and using GCP services like managing APIs, enabling billing and adding and removing collaborators and enabling other Google services. Each project is a separate compartment and each resource belongs to exactly one. Projects can have different owners and users - they're built separately and they're managed separately. Each GCP project has a name and a project ID that you assign. The project ID is a permanent, unchangeable identifier and it has to be unique acr...

## Hierarchy policies

* The policies implemented at a higher level in this hierarchy can't take away access that's granted at a lower level. For example, suppose that a policy applied on the bookshelf project gives user Pat the right to modify a cloud storage bucket, but a policy at the organization level says that Pat can only view cloud storage buckets not change them. The more generous policy is the one that takes effect. Keep this in mind as you design your policies.
