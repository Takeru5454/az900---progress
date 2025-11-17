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
    - Container Instances - Fastest and simplest way to run container in Azure. They are a PaaS.
    - Container Apps - 








  
