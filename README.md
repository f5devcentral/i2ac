# Infrastructure 2.0 as Code (I2aC)

## Executive Summary
Infrastructure 2.0 as Code (I2aC) is the ability to model your dynamic infrastructures as software, and then manage the infrastructure as a software project. F5 BIG-IPs are perhaps the most dynamic devices in the network, and I2aC provides a management modality that keeps up with the dynamic configuration and ongoing operations of our platform. Using I2aC unlocks the last 20 years of software development principles and best practices, such as Agile and collaborative programming. Managing your infrastructure as code provides the following benefits for your infrastructure and F5 BIG-IP devices: repeatability, automation, agility, scalability, reassurance, and disaster recovery.


## Introduction
“Software is eating the world” was a phrase coined by Netscape founder and venture capitalist Marc Andreesen in a Wall Street Journal article on August 20, 2011. It is an apt description of what is happening in networking, data centers and at F5 Networks today. In short, infrastructure has never been more dynamic or programmable. Infrastructure 2.0 is a synonym for these new dynamic IT infrastructures ; modeling them in code is the future.  Programmability is rapidly becoming the recommended approach to configure and orchestrate a BIG-IP device. Gone are the days of using the GUI or the CLI to manually massage a device into existence. 

Software is simply too hungry, its eating up every industry and creating hundreds if not thousands of application services at companies both small and large.  The average engineer or admin has simply too many complex applications to care for, and cannot keep up, without programmatic automation. Infrastructure 2.0 as Code (I2aC) is an answer to this problem. By using modern software development best practices and dynamic infrastructure approaches, engineers can leverage advanced programmability capabilities and configure and control their network and data center infrastructures. 

This blog article discusses the modern dynamic IT infrastructure, the benefits of managing your infrastructure as a software development project, and the importance of collaborative automation. It also summarizes and cites from industry the best practices and key recommendations of this important movement. 


## What is Infrastructure 2.0 as Code (I2aC)
Infrastructure as Code (IaC) is a 10-year-old practice of DevOps. It is arguably the most important one. It is the linchpin in a modern dynamic infrastructure. The value of Infrastructure as Code can be broken down into three, measurable categories: 
•	Cost (reduction)
•	Speed (faster execution)
•	Risk (remove errors and security violations) 

It has allowed organizations large and small to scale and achieve velocity across their infrastructure portfolios by modeling their infrastructures as software, and then managing those models as software projects. It has been said that DevOps is 90% culture and 10% tools. This paper is a call to arms to get network administrators and engineers using modern IaC approaches, and collaborative automation techniques. 

Puppet, an IaC company produces a State of DevOps report every year. Key findings from the report for 2016 survey were 
•	High-performing organizations deploy 200x more frequently
•	Recover 24x faster from failures
•	Have 2,555x shorter lead times
•	Have 3x lower change failure rates than low-performing ones

They also enjoy better
•	Employee loyalty (as measured by Net Promoter Scores)
•	Spend 22 percent less time on unplanned work and rework
•	Spend 50 percent less time remediating security issues
•	Benefit from an experimental approach to product development
•	Achieve significant cost savings from a (DevOps-driven) technology transformation. 

Treating infrastructure as code is a key element of DevOps, and it benefits both dev and ops teams. This new dynamic infrastructure approach is sweeping through the fields of network administration and engineering. IaC is one of the cornerstones of DevOps. It is the “A” in the DevOps tenets of “CAMS”: Culture, Automation, Metrics, and Sharing.  It is DevOps’ cornerstone, its foundation, its mainstay. Simply put, without automation there would be no DevOps. It provides a software development driven “operating system” for managing virtualized and bare-metal resources as software development projects. In today’s cloudy world we no longer need to build and maintain a few devices by hand, we need to be able to provision and manage hundreds if not thousands of servers and BIG-IPs and configure and orchestrate them in an automated and as collaborative a way as possible. 


## Dynamic Infrastructures
IaC can be leveraged to build and manage self-building, self-configuring, and self-healing network and server infrastructures. Modeling your infrastructure in code allows you to build or rebuild it with incredible speed. Utilizing dynamic Infrastructure 2.0 approaches reduces cost, increases speed, and minimizes risk. IaC eliminates configuration drift by providing a Source of Truth for the network and server infrastructure. Making this Source of Truth dynamic allows administrators and engineers to future proof their environments and infrastructure investments, prepare for the increasing dynamic requirements of containers and micro-services, and keep up with the velocity and scale requirements of the latest fast paced software project. 

Dynamic inventories allow I2aC to query and register with a dynamic data source for host inventory configuration information. Service discovery is the automatic detection of devices on a computer network. Tools such as Hashicorp’s Consul can be leveraged to automatically discover and then register servers with a service registry database.  This service registry can be leveraged by I2aC to automatically configure the network and server infrastructure. Web hosts can automatically add and remove themselves to Consul and I2aC can then use that information to automatically add and remove nodes from a pool on a BIG-IP. This powerful use case can be further expanded with dynamic infrastructure-aware variables.

Dynamic variables provide dynamic configuration. All IaC tools have a concept of “facts about the system”. Facts are dynamic variables representing system information, such as a devices IP address or CPU information. They allow IaC to dynamically configure a device such as a BIG-IP. For example, a “fact” that runs the tmsh command **show /sys hardware** could be used to automatically configure a dev, qa, pre-prod, or prod BIG-IP environment based on the hardware platform being configured. In other words, a pair of i2600 BIG-IPs could be automatically configured for dev duty, while a pair of i7800s could be automatically configured for prod. What makes this possible are the dynamic platform “facts” about the system. A little bit of self-awareness, or artificial intelligence goes a long way and can allow you to build self-building, self-configuring, and self-healing dynamic next generation infrastructures. 


## Collaborative Automation
Collaborative automation is simply teams of engineers and administrators working together, towards a common goal, utilizing automation tooling to make their jobs easier, more efficient, and stress free. A secondary DevOps practice configuration management is important to I2aC, and has undergone a fundamental shift over the last few years as social coding via sites like github.com have become increasingly popular. Network teams are able to share their software modeled BIG-IPs with other team members, solicit feedback, find bugs, and squash those bugs all because their BIG-IPs are modeled in code. 

"Agile is about embracing change, treating it as an expected thing, and even a positive, as opposed to old-school, viewing change as a problem," says Kief Morris. "If you use automation tools but still manage your infrastructure with the Iron Age approaches to change management, you’re losing the benefit. IAC is more reliable, particularly if you use Agile engineering practices like test driven development, continuous integration and continuous delivery." 

Learning and understanding how to manage your infrastructure and BIG-IP’s as a software project is incredibly valuable. Software development has reached a level of maturity allowing its techniques to be utilized in fields such as network engineering. An I2aC project can be managed via Agile methodologies such as Scrum and Kanban.  This allows engineers to coordinate and manage their infrastructures with agility and achieve project velocity. Social coding techniques such as peer review increase the quality of the I2aC software. Automated tests can be run against the I2aC software, finding defects and alerting engineers to bugs found. As I2aC software development maturity increases, there will be fewer bugs, but most importantly project velocity will increase and the network and ADC environment will keep pace with the velocity of the ever-increasing software projects they are meant to support. 


## A Call to Arms
Now is the time to get involved and learn Infrastructure 2.0 as Code. An infrastructure automation tool such as Ansible is easy to learn and use thanks to its simplified design and approach. “Ansible is a radically simple IT automation platform that makes your applications and systems easier to deploy. Avoid writing scripts or custom code to deploy and update your applications— automate in a language that approaches plain English, using SSH, with no agents to install on remote systems”. F5 Networks has created a demonstration and learning environment utilizing Docker. This “F5 Super NetOps” Docker environment downloads F5 Network’s Ansible best practice based example code base. The combination of the Docker demo/learning environment and the Ansible code will surely get a new I2aC practitioner on their way to freedom from the GUI and CLI and allow them to take advantage of all the benefits of Infrastructure 2.0 as Code.  These benefits are exemplified in the practices of infrastructure as code by Stephen Nelson-Smith. They are:
•	Repeatability – The very act of modeling your infrastructure in code provides repeatability. Every configuration element is captured in the code and the IaC tool will enforce that defined configuration each and every time it is run. IaC provides confidence that the infrastructure is configured and operating in the way it is supposed to be. 
•	Automation – The very act of abstracting out infrastructures brings us the benefits of automation. 
•	Agility – Utilizing collaborative automation techniques like configuration management provide a confidence in the various versions of the IaC code base. This allows an engineer or administrator to roll forward or backward if a problem were encountered. Logs of who did what when are available and can be analyzed to determine who or what caused the problem. This minimizes the average time to fix problems and encourages root cause analysis.
•	Scalability – Repeatability plus automation makes scalability much easier, especially when combined with the rapid hardware provisioning that the cloud provides.
•	Reassurance – The fact that the architecture, design, and implementation of our infrastructure is modeled in code means we that we can automatically have documentation. Any programmer can look at the source code and see at a glance who the systems work. This is a welcome change from the common scenario in which only a s single sysadmin or architect holds the understanding of how the system hangs together. That is risky- this person is now able to hold the organization ransom, and should they leave or become ill, the company is endangered.
•	Disaster Recovery – In the event of a catastrophic event that wipes out the production systems, if your entire infrastructure has been broken down into modular components and described as code, recovery is as simple as provisioning new compute power, restoring from backup, and deploying the infrastructure and application code. What may have been a business ending event in the old paradigm of custom-built, partially automated infrastructure becomes a manageable few hour outage, potentially delivering competitive value over those organizations suffering from the same external influences, but without the power and flexibility brought about by infrastructure as code.


To run the F5 Super NetOps Docker container and automatically download the best practices code base, issue the following command:


**docker run -p 8080:80 -p 2222:22 --rm -it -v user_repos.json:/tmp/user_repos.json -e SNOPS_GH_BRANCH=develop f5devcentral/f5-super-netops-container:develop-ansible**



The above commnd requires the user_repos.json file which is a config file that tells the Docker container where to find the best practices based Ansible code base. 

user_repos.json file example:

**{
  "repos": [
    {
      "name":"ansible_f5",
      "repo":"https://github.com/F5devcentral/ansible_f5.git",
      "branch":"master",
      "skip":false,
      "skipinstall":true
    }
  ]
}**

## Conclusion
Managing your infrastructure as code is very beneficial, it provides: repeatability, automation, agility, scalability, reassurance, and disaster recovery. All of which are incredibly important to a modern, dynamic infrastructure. Software development best practices are key to scaling and managing the modern dynamic data center, and I2aC provides a platform for turning your infrastructure organization into a modern, agile one. The ability to move and pivot your infrastructure quickly is now a requirement for most organizations. 



                                          **Works Cited**
Nelson-Smith, Stephen. "Chapter 1." Test-driven Infrastructure with Chef. Beijing: O'Reilly, 2013. 
https://en.wikipedia.org/wiki/Dynamic_infrastructure
 https://en.wikipedia.org/wiki/Infrastructure_as_Code
 https://puppet.com/resources/whitepaper/2016-state-of-devops-report
 https://info.microsoft.com/WE-Azure-CNTNT-FY16-05May-09-Forrester-Report-Infrastructure-As-Code-Fueling-The-Fire-For-Faster-Application-Delivery.html
  http://www.cio.com/article/3017722/infrastructure/what-is-infrastructure-as-code-and-why-should-you-embrace-it.html
https://github.com/ansible/ansible


