[practice-exam-3.md](https://github.com/user-attachments/files/31232383/practice-exam-3.md)

# AZ-900 Practice Exam 3 --- Lessons 16--20

This practice exam covers the concepts introduced in **Lessons 16--20**.

### Topics Covered

-   Azure Policy, Policy Definitions, Initiatives, Assignments, and
    compliance
-   Resource Locks, Tags, and Azure RBAC comparisons
-   Cloud Adoption Framework and governance hierarchy
-   Microsoft Purview, Trust Center, compliance documentation, and
    sovereign environments
-   Microsoft Defender for Cloud, Secure Score, Defense in Depth, and
    Zero Trust
-   Network Security Groups, Azure Firewall, Azure DDoS Protection, and
    Azure Key Vault
-   Microsoft Sentinel, Azure Dedicated Hosts, encryption, secrets,
    certificates, and Identity Protection
-   Azure costs, Pricing Calculator, TCO Calculator, Cost Management,
    SLAs, service lifecycle, Reservations, and Spot VMs

> \[!IMPORTANT\] Try to complete the exam without using your lesson
> notes, glossary, cram sheet, comparison tables, or answer key.

------------------------------------------------------------------------

# 📋 Instructions

-   **40 questions**
-   Choose the **best answer** unless the question says **Choose two**.
-   Suggested time: **45--60 minutes**
-   Suggested passing target: **80%**
-   Each question is worth **1 point**.
-   Maximum score: **40 points**

``` text
36–40 = Excellent
32–35 = Ready to move forward
28–31 = Review weak areas
 0–27 = Revisit Lessons 16–20
```

------------------------------------------------------------------------

# Questions

## 1.

An organization requires all new Azure resources to be deployed only in
approved regions.

Which Azure feature best fits this requirement?

A. Azure RBAC\
B. Azure Policy\
C. Resource Lock\
D. Tag

------------------------------------------------------------------------

## 2.

What is an individual rule in Azure Policy called?

A. Initiative\
B. Assignment\
C. Policy Definition\
D. Resource Lock

------------------------------------------------------------------------

## 3.

An organization wants to group several related Policy Definitions
together for a common governance goal.

What should it create?

A. Initiative\
B. Tag\
C. Resource Lock\
D. Azure RBAC role

------------------------------------------------------------------------

## 4.

What applies a Policy Definition or Initiative to a particular Azure
scope?

A. Secure Score\
B. Policy Assignment\
C. Resource Tag\
D. Service Level Agreement

------------------------------------------------------------------------

## 5.

A production database must be protected from accidental deletion, but
authorized administrators should still be able to modify it.

Which lock best fits?

A. ReadOnly\
B. CanNotDelete\
C. Azure Policy\
D. Contributor

------------------------------------------------------------------------

## 6.

A critical resource must not be modified or deleted through Azure
management operations.

Which lock should be used?

A. CanNotDelete\
B. ReadOnly\
C. Reader\
D. Policy Definition

------------------------------------------------------------------------

## 7.

A company wants to label resources with values such as
`Department=Finance` and `Environment=Production`.

Which feature should it use?

A. Tags\
B. Azure RBAC\
C. Azure Firewall\
D. Azure Policy Initiative

------------------------------------------------------------------------

## 8.

Which statement correctly compares Azure RBAC and Azure Policy?

A. RBAC controls resource configuration; Policy controls passwords.\
B. RBAC controls who can perform actions; Policy controls what
configurations are allowed or required.\
C. RBAC and Policy perform the same function.\
D. Policy controls user permissions; RBAC provides resource labels.

------------------------------------------------------------------------

## 9.

A company wants structured guidance for planning, preparing, adopting,
governing, securing, and managing its cloud journey.

Which resource best fits?

A. Cloud Adoption Framework\
B. Azure Firewall\
C. Microsoft Sentinel\
D. Azure Pricing Calculator

------------------------------------------------------------------------

## 10.

Which service is primarily associated with discovering, understanding,
and governing organizational data?

A. Microsoft Purview\
B. Azure Advisor\
C. Azure DDoS Protection\
D. Azure App Service

------------------------------------------------------------------------

## 11.

A customer wants information about Microsoft's security, privacy, and
compliance practices.

Which resource should the customer review?

A. Microsoft Trust Center\
B. Azure Monitor\
C. Azure Marketplace\
D. Azure Resource Manager

------------------------------------------------------------------------

## 12.

A regulated organization wants to determine which compliance standards
and offerings are supported by Azure.

Which resource is the best fit?

A. Azure Compliance Documentation\
B. Azure Pricing Calculator\
C. Azure Service Health\
D. Azure Key Vault

------------------------------------------------------------------------

## 13.

A government organization requires a specialized cloud environment
designed for sovereignty, isolation, compliance, and data-residency
requirements.

Which concept best fits?

A. Public Preview\
B. Sovereign Azure environment\
C. Azure Resource Group\
D. Azure Reservation

------------------------------------------------------------------------

## 14.

A legal team wants to understand Microsoft's commitments for processing
and protecting customer data.

Which document is most relevant?

A. Data Protection Addendum (DPA)\
B. Azure Policy Definition\
C. SLA\
D. Resource Lock

------------------------------------------------------------------------

## 15.

Which statement about Azure Blueprints matches the Lesson 17 material?

A. It is the primary current service for Azure network security.\
B. It is a legacy governance concept and should not be a major current
hands-on focus.\
C. It replaces Microsoft Purview.\
D. It is required for every Azure subscription.

------------------------------------------------------------------------

## 16.

Which service provides cloud security posture management and workload
protection capabilities?

A. Microsoft Defender for Cloud\
B. Azure DNS\
C. Azure Files\
D. Azure Pricing Calculator

------------------------------------------------------------------------

## 17.

Which Defender for Cloud feature provides a numerical measurement that
helps assess security posture?

A. Secure Score\
B. Resource Lock\
C. SLA\
D. Tag

------------------------------------------------------------------------

## 18.

A security architecture uses physical, identity, perimeter, network,
compute, application, and data protections so that multiple security
layers protect the workload.

Which security concept is this?

A. Zero Trust\
B. Defense in Depth\
C. Azure RBAC\
D. Public Preview

------------------------------------------------------------------------

## 19.

Which security model is based on principles including **Verify
Explicitly**, **Use Least Privilege Access**, and **Assume Breach**?

A. Defense in Depth\
B. Zero Trust\
C. Resource Locking\
D. High Availability

------------------------------------------------------------------------

## 20.

Which statement best describes the Zero Trust approach?

A. Trust requests from inside the corporate network automatically.\
B. Trust administrators but verify regular users.\
C. Do not automatically trust a request based only on its location.\
D. Allow all traffic unless an NSG denies it.

------------------------------------------------------------------------

## 21.

A company needs simple allow/deny rules controlling inbound and outbound
traffic for Azure subnets and network interfaces.

Which feature should it use?

A. Network Security Group\
B. Azure Key Vault\
C. Microsoft Sentinel\
D. Azure Dedicated Host

------------------------------------------------------------------------

## 22.

An organization wants a centralized managed firewall for Azure network
traffic.

Which service should it use?

A. Network Security Group\
B. Azure Firewall\
C. Azure DDoS Protection\
D. Microsoft Purview

------------------------------------------------------------------------

## 23.

A public-facing application is being targeted by a large-scale
traffic-flood attack.

Which service is designed to help mitigate this type of attack?

A. Azure Firewall\
B. Azure DDoS Protection\
C. Azure Key Vault\
D. Microsoft Sentinel

------------------------------------------------------------------------

## 24.

An application needs a secure location to store database passwords, API
keys, cryptographic keys, and certificates.

Which service should be used?

A. Azure Key Vault\
B. Azure Monitor\
C. Azure Policy\
D. Azure Advisor

------------------------------------------------------------------------

## 25.

What does **encryption** primarily protect against?

A. Accidental deletion\
B. Unauthorized reading of data\
C. High Azure costs\
D. DDoS attacks

------------------------------------------------------------------------

## 26.

A security operations team needs a cloud-native SIEM to collect,
analyze, investigate, and respond to security events.

Which service should it use?

A. Microsoft Sentinel\
B. Azure Key Vault\
C. Azure Policy\
D. Microsoft Purview

------------------------------------------------------------------------

## 27.

A regulated workload requires Azure VMs to run on physical server
capacity dedicated to one customer.

Which Azure offering best fits?

A. Azure Dedicated Host\
B. Azure Functions\
C. Azure Spot Virtual Machines\
D. Azure Container Instances

------------------------------------------------------------------------

## 28.

A security team wants to identify risky users and suspicious sign-ins.

Which service best fits?

A. Microsoft Entra ID Protection\
B. Azure Firewall\
C. Azure DDoS Protection\
D. Azure Cost Management

------------------------------------------------------------------------

## 29.

An administrator creates two NSG rules. One has priority **200** and the
other has priority **300**.

Which rule is evaluated first?

A. Priority 300\
B. Priority 200\
C. Both are evaluated simultaneously\
D. Priority does not affect evaluation

------------------------------------------------------------------------

## 30.

Which tool should be used to estimate the expected monthly cost of a
Virtual Machine **before** it is deployed?

A. TCO Calculator\
B. Azure Pricing Calculator\
C. Secure Score\
D. Azure Service Health

------------------------------------------------------------------------

## 31.

A company wants to compare the cost of its current on-premises servers,
storage, networking, electricity, and labor with moving those workloads
to Azure.

Which tool should it use?

A. Azure Pricing Calculator\
B. TCO Calculator\
C. Azure Advisor\
D. Microsoft Sentinel

------------------------------------------------------------------------

## 32.

Which Azure service helps an organization monitor, analyze, and optimize
its cloud spending after resources are in use?

A. Azure Cost Management\
B. Azure Policy\
C. Azure Monitor\
D. Microsoft Purview

------------------------------------------------------------------------

## 33.

Which of the following can affect the cost of an Azure resource?

A. Region\
B. Resource type\
C. Usage duration\
D. All of the above

------------------------------------------------------------------------

## 34.

What is an Azure Service Level Agreement (SLA)?

A. A resource labeling system\
B. Microsoft's availability commitment and associated terms for an Azure
service\
C. A method of granting user permissions\
D. A tool for estimating on-premises costs

------------------------------------------------------------------------

## 35.

What may be available when Microsoft fails to meet an eligible service's
SLA terms?

A. A Service Credit\
B. A Resource Tag\
C. A Policy Initiative\
D. A Dedicated Host

------------------------------------------------------------------------

## 36.

Which service lifecycle stage is fully released and generally
appropriate for production use?

A. Private Preview\
B. Public Preview\
C. Generally Available (GA)\
D. Retired

------------------------------------------------------------------------

## 37.

Which statement best describes a **Public Preview** service according to
Lesson 20?

A. It is fully released and backed like a GA service.\
B. It is broadly available for evaluation but may have limited support
and is not intended as the default choice for critical production
workloads.\
C. It is available only to Microsoft employees.\
D. It has been retired.

------------------------------------------------------------------------

## 38.

A company has a predictable long-running Azure workload and is willing
to make a commitment in exchange for potential cost savings.

Which purchasing option best fits?

A. Azure Reservation\
B. Azure Spot Virtual Machine\
C. Public Preview\
D. Azure DDoS Protection

------------------------------------------------------------------------

## 39.

A batch-processing workload can tolerate interruption and the company
wants discounted unused Azure compute capacity.

Which option best fits?

A. Azure Reservation\
B. Azure Spot Virtual Machine\
C. Azure Dedicated Host\
D. ReadOnly Lock

------------------------------------------------------------------------

## 40. Choose two.

Which **TWO** statements correctly compare Azure Reservations and Azure
Spot Virtual Machines?

A. Reservations are designed for eligible predictable workloads where a
commitment can provide savings.\
B. Spot VMs can be evicted when Azure needs the capacity.\
C. Reservations are designed primarily for workloads that must be
interrupted without notice.\
D. Spot VMs provide dedicated physical hardware for one customer.

------------------------------------------------------------------------

# 🛑 Stop Here

Do not open `answer-key-3.md` until you have completed all 40 questions.

Record your answers:

``` text
 1. ____    11. ____    21. ____    31. ____
 2. ____    12. ____    22. ____    32. ____
 3. ____    13. ____    23. ____    33. ____
 4. ____    14. ____    24. ____    34. ____
 5. ____    15. ____    25. ____    35. ____
 6. ____    16. ____    26. ____    36. ____
 7. ____    17. ____    27. ____    37. ____
 8. ____    18. ____    28. ____    38. ____
 9. ____    19. ____    29. ____    39. ____
10. ____    20. ____    30. ____    40. ____
```

When finished, compare your answers with **`answer-key-3.md`**.
