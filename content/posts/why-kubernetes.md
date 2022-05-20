---
title: "So, Why Kubernetes?"
date: 2022-05-20T15:15:31+01:00
draft: false
---

## The hidden reasons that drive technology adoption.

Kubernetes has been groundbreaking as an all-in-one solution for managing service discovery, network flows/policies, scalability, and container lifecycle. Now, you don't necessarily need all of these things when your current stack already effectively meets your business needs. Therefore, adopting Kubernetes for its most notable qualities is not always the primary reason.

I recently worked for a company that was already happy with their existing stack – a simple monolithic application running on a few ec2 instances. However, they needed to automate the creation of ephemeral environments for each new pull request. To do this, the current infrastructure involved dynamically provisioning the virtual machines where the code would be built and executed, while resolving inter-service communication and managing the routing of external traffic via an application load balancer. All of this can quickly become a tedious process, overburdened compared to other platforms that natively cover all of these features.

Of the many solutions that could meet their needs, Kubernetes is quickly emerging as the most pragmatic, as the number of online resources advocating its use has significantly reinforced existing assumptions, acting as a proxy for confirmation bias. However, could another less popular option be better? Sometimes following the hype is not unnecessarily an irrational decision, in the case of adopting Kubernetes, there is an established community that can dramatically reduce the learning curve while reducing the magnitude of its complexity, and the more you can leverage its utility, the faster a mature operational state can be reached. Additionally, the hiring argument weighs heavily on your decisions because, in some cases, not being able to scale your engineering department can be much worse than not scaling your infrastructure.

Nevertheless, migrating to Kubernetes can have a significant operational cost while important aspects are often overlooked, such as defining the stack observability holistically, enabling scalability at multiple levels, choosing the right CNI, and managing cluster upgrades, not to mention transferring knowledge down the chain. Of course, some of these technical details can be abstracted with newer, highly managed solutions that have entered the market - knative is a good example. While the adoption of these hybrid serverless solutions continues to grow, many of their promises only partially address the complexity that many organizations face due to oversimplification.

Finally, Kubernetes is far from the only example as many companies often make decisions as a result of adopting trendy, cutting-edge technologies when the underlying reasons may be different from what the chosen product officially stands for. And, more often than not, technical solvency is overvalued in the face of other important factors such as operational costs, long-term maintainability, community presence, hiring perspectives, and so on.
