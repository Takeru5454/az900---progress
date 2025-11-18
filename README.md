# az900---progress
Notes for Microsoft Azure Fundamentals Certification

PART 1: CLOUD CONCEPTS
  IaaS (Infrastructure as a Service) - Places most responsibility on the consumer
    - Lift and Shift Migration - Moving existing application and its data to cloud without changing code
    - Testing and Development - Start up or shut down different environments while maintaining control
  PaaS (Platform as a Service) - Evenly distributes responsibility
    - Development Framework - Pre-built tols and environments that help devs test apps without managing infrastructure
    - Analytics or Business Intelligence - Analyse data to find patterns to predict outcomes
  SaaS (Software as a Service) - Places most responsibility on the cloud provider
    - Least flexible but easiest to get up and running
    - Common Scenarios - | Email and messaging | Business productivity applications | Finance and expense tracking |

  Uptime (High Availability) - Ensure availability, regardless of disrptions or events
  Scalability (Handle Demand) - Ability to adjust resources to meet demand
    - Vertical Scaling - Add more CPUs or RAM to VM
    - Horizontal Scaling - Add more VMs

  Reliability - Recover from failures and continue to function
  Performance Predictability - Predicts resources needed to keep uptime and ensure smooth, consistent performance
  Cost Predictability - Predict future costs and track resource use in real time
  
  CLOUD MODELS:
    Private Cloud - Cloud that is hosted and used by a single organization which provides greater control but with greater cost and fewer public cloud benefits
      - Hosted in a datacenter
      - Healthcare, Government may need stricter security or very specific configs
    Public Cloud - CLoud that is hosted and managed by external providers like AWS, Azure, or GCP, and shared across many organizations.
      - Less control over management and updates
      - Sensitive data may be less secure
      - Access to tools without managing backend
    Hybrid Cloud - Cloud that uses both public and private cloud
      - Required to manage two environments which may increase costs
      - Great flexibility with security, agility and scalability
    Multi-CLoud - Use and manage two or more public cloud providers

  
PART 2: AZURE COMPUTE AND NETWORKING SERVICES
  Virtual Desktop - Enables you to use a cloud-hosted version of windows from any location
    - Enhanced Security - Enable multifactor authentication, assign granular role-based access controls
       - The data and apps are separated from the local hardware. The actual desktop and apps are running in the cloud, meaning the risk of confidential data being left on a personal device is reduced
  Containers -  lightweight, portable packages of software that run consistently across environments
    - Bundles your application code with all its dependencies (libraries, runtime, configs) so it runs the same everywhere
    - Container Instances - Fastest and simplest way to run container in Azure. They are a PaaS. You dont have to manage any VMs
    - Container Apps - Similar to Instances but they allow you to incorporate load balancing and scaling
    - Kubernetes Service - Makes managing containers simpler and more efficient
  Functions - Serverless option that doesn’t require maintaining virtual machines or containers
    - Used when you need to perform work in response to an event and when that work can be completed within seconds or less
    - Scales automatically - good choice when demand is variable
  Azure App Service - Enables you to build and host web apps, background jobs, mobile back-ends, and RESTful APIs in any programming language without managing infrastructure
    - Common Apps - Web apps, API apps, WebJobs, Mobile apps
    - Deployment and management are integrated into the platform. Endpoints can be secured. Sites can be scaled quickly to handle high traffic loads. The built-in load balancing and traffic manager provide high availability.

  Virtual Networks - Enables VMs, web apps, and databases to communicate with each other
    Virtual networks can connect not only VMs but other Azure resources
    Key networking capabilities:
      - Isolation and segmentation
      - Internet communications
      - Communicate between Azure resources
      - Communicate with on-premises resources
      - Route network traffic
      - Filter network traffic
      - Connect virtual networks
    Supports both public and private endpoints to enable communication between external or internal resources with other internal resources
      - Public endpoints have a public IP address and can be accessed from anywhere in the world
      - Private endpoints exist within a virtual network and have a private IP address from within the address space of that virtual network
    Isolation - You define a private IP address and it only exists within the virtual network and it isnt internet routable
    Internet Communications - Assign a public IP address to an Azure resource, or putting the resource behind a public load balancer
    








  
