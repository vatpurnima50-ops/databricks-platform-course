warehouse: used by BI to query the tables and all, it contain structured data but expensive but reliable, not supports raw data, streaming data
data lake: like your S3 where you can store raw data but no acid guarantee, efficient, cheap, useful for ML workloads
lakehouse; Build a table layer on top of S3 which can make it schema enforcement acid gurantee, transaction logs and and provide versioning alonhg with time travel
now if you have data warehouse and data lake which make make multiple copies of single data file which can ater makes conflict and which cause data drift as well so to avoid this data lakes keeps a single copy on S3
and make table layer on top of it


Platform admin Charter:
1. Access: Grant access to user, groups and creating them as well
2. Security: Creating IAM Roles, Encryption Settings, VPC rules
3.Cost: Setting up a budget, Creating A Budget Alerts which means cost Guardrails
4. Reliability: Quotas, Workspace Deployment, Incidents
5. Delivery:  Repeatable environments in terraform


