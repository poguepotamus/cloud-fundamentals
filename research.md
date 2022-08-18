# Course research

## Course Standards

1. Understand the characteristics of cloud computing from a business perspective
2. Understand the business value of cloud computing
3. Differentiate between cloud types and the technical challenges presented by each type
4. Understand the steps to successful adoption of cloud computing
5. Understand the impact and changes of cloud computing in IT management
6. Discuss the risks and consequences of cloud computing

### Hosting

What is a [hypervisor](https://en.wikipedia.org/wiki/Hypervisor)?

> A hypervisor is a elevated supervisor (kernel) to manage many operating systems and distrubute resources among them.

There are a two types of hypervisors (hv), type 1 and type 2. We'll also review containers because they are conceptually similar, though they have a very different use case.

### Type 1 HV's

Are considered 'native' hosted HV's as they have their hypervisor directly installed on the hardware. This allows for the best case scenario when allocating resources and reducing overhead processing.

Examples:
- Hyper-V
- ESXi
- KVM
- Red Hat Virtualization

### Type 2 HV's

A HV installed on an OS. There are many different forms, but typically the HV will share the kernal of the host system.

- Workstation
- Oracle VM (vbox)
- Parallels
- Fusion

### Containers

Does not setup an OS to run applications, but creates a sterile environment to do so. This also uses the host kernel

> Running applications that can't use the host's kernel is common, in most cases the container server will install and run a VM that can host the container.

[![Useful graphic for different hypervisors](https://i.stack.imgur.com/HZ34i.png)](https://stackoverflow.com/questions/6044978/full-emulation-vs-full-virtualization)

[![How containers use os-specific containers](https://docs.microsoft.com/en-us/virtualization/windowscontainers/deploy-containers/media/mobyvm.png)](https://docs.microsoft.com/en-us/virtualization/windowscontainers/deploy-containers/linux-containers)


## Cloud Service Models

### On Premises

For comparison, lets look at what you can expect to manage if you're hosting the service yourself.

Process stack:

- Application
- Data
- Runtime
- Middleware
- Operating System
- Virtualization
- Networking
- Storage
- Servers

### IaaS - Infrastructure as a Service

Takes care of the following layers:

- Virtualization
- Networking
- Storage
- Servers

### PaaS - Platform as a Service

Leaves this for you to take care of:

- Application
- Data

This is mainly used for development environments while coding something specific.

For example, RedHat's OpenShift PaaS that offers one-click deployments of many lanugage or framework development environments for any operating system.

### SaaS - Software as a Service

More of a software distrobution model. Makes an application available over the Internet.

#### Examples:

- Email clients
  - gmail
  - office365
- Storage
  - Dropbox
  - Onedrive
- Misc
  - Salesforce
  - Discord
  - Slack
- Everyone's favorite: blackboard

### Recap

- Accessability
- Updates/patches
- Hardware
- General Maintaince
- Backups
- Shared resources
- Reduced cost

## Cooking as a Service Model

Ask for recipe, get ingredients. Remove them as a IaaS service model example

Remove the cooking phase as the PaaS example

Everything removed for dining out



## Cloud Computing Challenges

### Security

Between hacking and virusus, cyber-security is becoming one of the fastest growing industries because cloud options are increasing. Third-party companies are offering services to cloud computing companies for security updates.

### Managing Cloud Spending

Starting a cloud instance and forgetting about it, hidden fees, and other issues are causing companies to spend more than they intend on cloud spending.

### Lack of Expertise

Finding qualified employees to manage the cloud connections from a company

### Compliance

Compliance depends on the data that is being stored. Some data will have company policies that determine how it's handled, other data has laws that determine how it's handed. Knowing and following all the rules associated with each set of data is a challenge in itself.


## Cloud Security Alliance (CSA)

The [CSA](https://cloudsecurityalliance.org/) is made up of companies that deal with cloud computing and is dedicated to defining and rasing awareness of best practices to help ensure a secure cloud computing environment.

### Security Issues

- Data Breaches
- Misconfiguration and Inadequate Change Control
- Lack of Cloud Security Architecture and Strategy
- Insurfficient Identity, Redentials, and Access Management
- Account Hijacking
- Insider Threat
- Insecure Interfaces and APIs
- Weak Control Plane
- Metastructure and Applistructure Failures
- Limited Cloud Usage Visibility
- Abuse and Nefarius use of Cloud Services

[Egregious 11 release from 2020](The-Egregious-11-Cloud-Computing-Top-Threats-in-2019-April2020.pdf)