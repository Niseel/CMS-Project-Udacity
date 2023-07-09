# Write-up Template

### Choose, and justify the appropriate resource option for deploying the app.
- *My choice is App service*
- *Personally, I think the CMS app is quite simple, with the main task of saving records about the information of an article.* 
- *The right infrastructure for a CMS app is PaaS. It has all the dependencies supported, is quite easy to manage, and does not take too much time to configure from scratch like VMs (IaaS), so it can easily integrate with Azure Active Directory.*

### Analyze the appropriate resource option for deploying the app.
#### Cost
- *App Service:  App Services have a pay-as-you-go model based on usage. Suitable for small assignments or low-user applications like CMS.*
- *VMs: Virtual machines have a fixed cost based on size and configuration. Expensive for small apps like CMS.*

#### Scalability
- *App Service: Scalability is more easier if I choose App Service by it support automatic scaling when when the traffic reaches a certain threshold*
- *VMs: VMs are required manual scaling by IT, Devops*

#### Availability
- *App Service: With built-in load balancing and fault tolerance i believe App Service is strong in Availability*
- *VMs: Virtual machines require more management and maintenance. But this is also the point and necessity of VMs compared to App Service when the manager has more rights and autonomy.*

#### Workflow
- *App Service: Easier to install and use With Azure Portal config*
- *VMs: As a IaaS itself, the installation will require a few more steps after initializing the virtual machine compared to the App Service*


### Assess app changes that would change your decision.
*For example, If my CMS Application becomes a super big application with 100 billion users a day, it might be necessary to consider migrating from Azure App Service to virtual machines (VMs) for better scalability, availability, and cost management. Let me give you some example to support my opinion*

#### Cost
*App Service is not the most cost-effective option for extremely high traffic scenarios. VMs provide more flexibility in terms of resource allocation and can be more cost-efficient for handling large-scale applications.*

#### Scalability
*As my CMS grows to accommodate 100 billion users a day, I'll need a highly scalable infrastructure. VMs allow me to scale horizontally by adding more instances to handle increased traffic. With VMs, I have more control over the scaling process and can optimize it based on my application's requirements. This flexibility enables me to handle the high demand efficiently.*

#### Availability
*VMs can provide higher availability compared to the App Service, especially when combined with Azure Availability Sets or Availability Zones. By distributing my VMs instances across multiple fault domains and update domains, I can ensure that my application remains available even in the event of hardware failures or planned maintenance.*

#### Workflow
*With VMs, I'll have more control over the underlying infrastructure, including OS configuration, networking, and load balancing because it is IaaS (Infrastructure as a Service). This increased control might require additional setup and management tasks, such as load balancers, configuring virtual networks, and monitoring tools*