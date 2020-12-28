# Salesforce Orgs

What is a Salesforce org?
- A container on Salesforce servers via multi-tenancy
- These containers are subject to limitations called *Governor Limits*

<br>

## Types

- **Production**: primary place of business.
- **Sandbox**: copy of production metadata and perhaps data: preparation for production. It can pass changes to production.
    - Full copy: all production data and metadata
    - Partial copy: subset of data and all metadata
    - Personal: no data, all metadata
- **Developer Edition**: separate instance with small storage and tighter limitations.

<br>

Note: Sandboxes do not get ongoing data from Production. They only get data at time of creation.

- **DX Scratch orgs**: meant for development but totally blank with no data or metadata. require packages of Salesforce metadata to be installed into them for functionality.

<br>

## Deployment from Sandbox or Scratch Org to Production

1. Change sets
    - configurable through the Setup menu
    - can be send to production org
2. Metadata deployments
    - Ant migration tool: allows package up changes for deployment
    - Tools: Force.com IDE and Metadata API


With advanced deployments tool we can get:
- Version control
- Packaging
- Dependencies (management)

<br><br>

---
### References
- [Salesforce Administration: The Big Picture](https://www.pluralsight.com/courses/salesforce-administration-big-picture)