# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
Costs: VMs tend to be more expensive, but have a lower up-front cost compared to buying and maintaining hard. App Service pricing is based on the type of App Service Plan you chose.
Scalability: VMs (IaaS) have lots of options for configurations in terms of OS, compute, RAM, storage, etc. The App Service tiers provide lesser memory and CPU cores and also less control of the underlying OS, but can be both vertically or horizontally scaled.
Availablity: VMs can be scaled to provide high availability. Although an App Service can too, there is not enough control of the servers to allow for design freedom.
Workflow: VMs are labor intensive due to having full control of the VM, whereas an App Service is a PaaS offering (limited lower level control). VMs support a wide variety of languages while an App Service has limited options.

Given the analysis/information above, I chose an App Service for the Article CMS app since this is a lightweight app (created as a project) that does not require a lot of processing power and does not have a lot of users (just one - me). App Service is also cheap (utilized Free tier).

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
VMs can be considered if many new features are planned to be added to the app, or if demand changes in a way that requires vertical scaling. Other reasons for potentially moving away from an App Service - user base increases drastically, or custom security policies are needed.