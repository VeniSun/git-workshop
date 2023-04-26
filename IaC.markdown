# Infrastructure as Code

## What is IaC?
Infrastructure as code is a way managing and provisioning of infrastructure through code instead of doing it through a manual process.  

With IaC, configuration files are created that contain your infrastructure specifications, which makes it easier to edit and distribute configurations. It also ensures that you provision the same environment every time. By codifying and documenting you configuration specifications, Iac aids configuration management and helps you to avoid undocumented, ad-hoc configuration changes. 

By using source control, like Git, we can ensure that we have version control of the IaC. It also makes it easier to track changes which can aid in troubleshooting. 

Using IaC is also the first step in automating infrastructure.

There are two ways of approaching IaC. 

**The Declarative approach:** defines the desired state of the system, including what resources you need and any properties they should have. Then an IaC tool willl configure them for you. This approach also keeps the state of your system objects so it makes taking down the infrastructure simpler to manage.

**The Imperative approach:** defines the specific commands needed to achieve the desired configuration. These commands need to be executed in the correct order. 

Many IaC tools use a declarative approach and will automatically provision the desired infrastructure. If you make changes to the desired state, a declarative IaC tool will apply those changes for you. An imperative tool will require you to figure out how those changes should be applied.

IaC tools are often able to operate in both approaches, but tend to prefer one approach over the other.

**Benefits of IaC**

Provisioning infrastructure has historically been a time consuming and costly manual process. Now infrastructure management has moved away from physical hardware in data centers, though this still may be a component for your organization, to virtualization, containers, and cloud computing.

With cloud computing, the number of infrastructure components has grown, more applications are being released to production on a daily basis, and infrastructure needs to be able to be spun up, scaled, and taken down frequently. Without an IaC practice in place, it becomes increasingly difficult to manage the scale of today’s infrastructure.

IaC can help your organization manage IT infrastructure needs while also improving consistency and reducing errors and manual configuration.
Benefits:

- Cost reduction
- Increase in speed of deployments
- Reduce errors
- Improve infrastructure consistency
- Eliminate configuration drift

**IaC tools**

Server automation and configuration management tools can often be used to achieve IaC. There are also solutions specifically for IaC.
These are a few popular choices:

- Chef
- Puppet
- Red Hat Ansible Automation Platform
- Saltstack
- Terraform
- AWS CloudFormation

Ansible Automation Platform can be used to provision operating systems and network devices, deploy applications, and manage configuration.

**Why does IaC matter for DevOps?**

IaC is an important part of implementing DevOps practices and continuous integration/continuous delivery (CI/CD). IaC takes away the majority of provisioning work from developers, who can execute a script to have their infrastructure ready to go.

That way, application deployments aren’t held up waiting for the infrastructure, and sysadmins aren’t managing time-consuming manual processes.

CI/CD relies on ongoing automation and continuous monitoring throughout the application life cycle, from integration and testing to delivery and deployment.

In order for an environment to be automated it needs to be consistent. Automating application deployments doesn’t work when the development team deploys applications or configures environments one way and the operations teams deploys and configures another way.

Aligning development and operations teams through a DevOps approach leads to fewer errors, manual deployments, and inconsistencies.

IaC helps you to align development and operations because both teams can use the same description of the application deployment, supporting a DevOps approach.

The same deployment process should be used for every environment, including your production environment. IaC generates the same environment every time it is used.

IaC also removes the need to maintain individual deployment environments with unique configurations that can’t be reproduced automatically and ensures that the production environment will be consistent.

DevOps best practices are also applied to infrastructure in IaC. Infrastructure can go through the same CI/CD pipeline as an application does during software development, applying the same testing and version control to the infrastructure code.