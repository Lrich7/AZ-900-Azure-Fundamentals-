[answer-key-3.md](https://github.com/user-attachments/files/31232393/answer-key-3.md)

# AZ-900 Practice Exam 3 --- Answer Key

Answer key for **Practice Exam 3 --- Lessons 16--20**.

> \[!TIP\] Review the explanation for every question you missed **or
> guessed on**. The goal is to understand why the correct Azure service
> or concept fits the requirement.

------------------------------------------------------------------------

# 📊 Score Guide

  Score          Percentage Recommendation
  ------------ ------------ ------------------------------------
  **36--40**       90--100% Excellent --- strong understanding
  **32--35**      80--87.5% Ready to move forward
  **28--31**      70--77.5% Review weak areas
  **0--27**       Below 70% Revisit Lessons 16--20

> \[!NOTE\] This score guide is for this training repository. It is not
> Microsoft's official AZ-900 exam scoring system.

------------------------------------------------------------------------

# ✅ Answer Key

    \#    Answer     Topic
  ---- ------------- --------------------------------
     1     **B**     Azure Policy
     2     **C**     Policy Definition
     3     **A**     Initiative
     4     **B**     Policy Assignment
     5     **B**     CanNotDelete Lock
     6     **B**     ReadOnly Lock
     7     **A**     Tags
     8     **B**     RBAC vs. Policy
     9     **A**     Cloud Adoption Framework
    10     **A**     Microsoft Purview
    11     **A**     Microsoft Trust Center
    12     **A**     Azure Compliance Documentation
    13     **B**     Sovereign Azure
    14     **A**     DPA
    15     **B**     Azure Blueprints
    16     **A**     Defender for Cloud
    17     **A**     Secure Score
    18     **B**     Defense in Depth
    19     **B**     Zero Trust
    20     **C**     Zero Trust
    21     **A**     NSG
    22     **B**     Azure Firewall
    23     **B**     DDoS Protection
    24     **A**     Key Vault
    25     **B**     Encryption
    26     **A**     Microsoft Sentinel
    27     **A**     Dedicated Host
    28     **A**     Entra ID Protection
    29     **B**     NSG Priority
    30     **B**     Pricing Calculator
    31     **B**     TCO Calculator
    32     **A**     Cost Management
    33     **D**     Cost Factors
    34     **B**     SLA
    35     **A**     Service Credit
    36     **C**     Generally Available
    37     **B**     Public Preview
    38     **A**     Reservation
    39     **B**     Spot VM
    40  **A and B**  Reservations vs. Spot VMs

------------------------------------------------------------------------

# 🧠 Explanations

## Questions 1--8 --- Lesson 16: Governance

### 1. B --- Azure Policy

Azure Policy enforces organizational standards and evaluates resource
compliance.

``` text
Policy = WHAT IS ALLOWED?
```

A requirement restricting resources to approved Azure regions is a
configuration rule, so Azure Policy is the best fit.

------------------------------------------------------------------------

### 2. C --- Policy Definition

A **Policy Definition** is an individual Azure Policy rule.

``` text
Definition = RULE
```

------------------------------------------------------------------------

### 3. A --- Initiative

An **Initiative** groups multiple Policy Definitions together toward a
common governance goal.

``` text
Initiative = GROUP OF POLICIES
```

------------------------------------------------------------------------

### 4. B --- Policy Assignment

A Policy Assignment applies a Policy Definition or Initiative to a
scope.

``` text
Definition = RULE
Initiative = GROUP
Assignment = APPLY TO SCOPE
```

------------------------------------------------------------------------

### 5. B --- CanNotDelete

A **CanNotDelete** lock allows authorized users to read and modify the
resource but prevents deletion.

------------------------------------------------------------------------

### 6. B --- ReadOnly

A **ReadOnly** lock prevents management changes and deletion.

  Lock            Read   Modify   Delete
  -------------- ------ -------- --------
  CanNotDelete    Yes     Yes       No
  ReadOnly        Yes      No       No

------------------------------------------------------------------------

### 7. A --- Tags

Tags are key-value metadata used to organize and categorize Azure
resources.

``` text
Environment = Production
Department  = Finance
Owner       = IT
```

Tags do **not** grant permissions.

------------------------------------------------------------------------

### 8. B --- RBAC vs. Policy

The key distinction is:

``` text
RBAC   = WHO CAN DO IT?
Policy = WHAT IS ALLOWED?
```

------------------------------------------------------------------------

# Questions 9--15 --- Lesson 17: Governance & Compliance

### 9. A --- Cloud Adoption Framework

The Cloud Adoption Framework provides guidance for an organization's
cloud journey.

The Lesson 17 material includes methodologies such as:

``` text
Strategy
Plan
Ready
Adopt
Govern
Secure
Manage
```

It is guidance rather than an Azure resource-enforcement mechanism.

------------------------------------------------------------------------

### 10. A --- Microsoft Purview

Microsoft Purview provides data-governance capabilities including
concepts such as data discovery, cataloging, classification, and
lineage.

``` text
Purview = UNDERSTAND + GOVERN DATA
```

------------------------------------------------------------------------

### 11. A --- Microsoft Trust Center

The Trust Center provides information about Microsoft's security,
privacy, and compliance practices.

``` text
Trust Center = MICROSOFT TRUST INFORMATION
```

------------------------------------------------------------------------

### 12. A --- Azure Compliance Documentation

Organizations use Azure Compliance Documentation to understand Azure
compliance offerings and certifications.

> Microsoft's compliance does not automatically make a customer's own
> workload compliant.

------------------------------------------------------------------------

### 13. B --- Sovereign Azure Environment

Sovereign or government environments address specialized requirements
involving government, sovereignty, compliance, isolation, and data
residency.

------------------------------------------------------------------------

### 14. A --- Data Protection Addendum

The **DPA** explains Microsoft's commitments regarding how customer data
is processed and protected.

``` text
DPA = CUSTOMER DATA PROTECTION / PROCESSING
```

------------------------------------------------------------------------

### 15. B --- Azure Blueprints Is Legacy

The Lesson 17 material treats Azure Blueprints as a **legacy governance
concept** rather than a major current hands-on focus.

------------------------------------------------------------------------

# Questions 16--20 --- Lesson 18: Security I

### 16. A --- Microsoft Defender for Cloud

Microsoft Defender for Cloud helps improve cloud security posture and
protect supported workloads.

``` text
Defender for Cloud
= SECURITY POSTURE + WORKLOAD PROTECTION
```

------------------------------------------------------------------------

### 17. A --- Secure Score

Secure Score measures security posture based on implemented security
controls and recommendations.

``` text
Secure Score = MEASURE SECURITY POSTURE
```

A high score does not guarantee that an environment is completely
secure.

------------------------------------------------------------------------

### 18. B --- Defense in Depth

Defense in Depth uses multiple layers of security.

The lesson identifies layers including:

``` text
Physical
Identity & Access
Perimeter
Network
Compute
Application
Data
```

``` text
Defense in Depth = MANY LAYERS
```

------------------------------------------------------------------------

### 19. B --- Zero Trust

The Lesson 18 material identifies three major Zero Trust principles:

``` text
VERIFY EXPLICITLY
USE LEAST PRIVILEGE ACCESS
ASSUME BREACH
```

------------------------------------------------------------------------

### 20. C --- Do Not Automatically Trust Based on Location

Zero Trust does not automatically trust a request simply because it
comes from inside a corporate network.

``` text
Zero Trust = NEVER TRUST, ALWAYS VERIFY
```

------------------------------------------------------------------------

# Questions 21--29 --- Lesson 19: Security II

### 21. A --- Network Security Group

NSGs use allow/deny security rules to control inbound and outbound
network traffic for supported Azure networking resources.

``` text
NSG = INBOUND / OUTBOUND RULES
```

------------------------------------------------------------------------

### 22. B --- Azure Firewall

Azure Firewall is a managed centralized network firewall.

``` text
NSG            = RESOURCE / SUBNET TRAFFIC RULES
Azure Firewall = CENTRAL FIREWALL
```

------------------------------------------------------------------------

### 23. B --- Azure DDoS Protection

DDoS Protection is designed to help protect against Distributed
Denial-of-Service traffic-flood attacks.

``` text
Firewall = FILTER TRAFFIC
DDoS     = TRAFFIC-FLOOD PROTECTION
```

------------------------------------------------------------------------

### 24. A --- Azure Key Vault

Azure Key Vault securely stores and manages:

-   Secrets
-   Cryptographic keys
-   Certificates

``` text
Key Vault = SECRETS + KEYS + CERTIFICATES
```

------------------------------------------------------------------------

### 25. B --- Unauthorized Reading of Data

Encryption converts readable information into an unreadable form to
protect it from unauthorized access.

``` text
Encryption = PROTECT DATA
```

------------------------------------------------------------------------

### 26. A --- Microsoft Sentinel

Microsoft Sentinel is the security operations / SIEM service covered in
Lesson 19.

**SIEM** stands for:

``` text
Security Information and Event Management
```

It helps security teams collect and analyze security events and
investigate/respond to threats.

------------------------------------------------------------------------

### 27. A --- Azure Dedicated Host

A Dedicated Host provides physical server capacity dedicated to one
Azure customer for supported Azure VMs.

``` text
Dedicated Host = DEDICATED PHYSICAL AZURE SERVER
```

------------------------------------------------------------------------

### 28. A --- Microsoft Entra ID Protection

Identity Protection focuses on identity-based risks such as risky users
and suspicious or risky sign-ins.

------------------------------------------------------------------------

### 29. B --- Priority 200

Lower NSG priority numbers are evaluated before higher priority numbers.

``` text
200 → evaluated before → 300
```

------------------------------------------------------------------------

# Questions 30--40 --- Lesson 20: Pricing & Support

### 30. B --- Azure Pricing Calculator

The Azure Pricing Calculator estimates the expected cost of Azure
resources before deployment.

``` text
Pricing Calculator = WHAT WILL AZURE COST?
```

------------------------------------------------------------------------

### 31. B --- TCO Calculator

The Total Cost of Ownership Calculator compares current on-premises
costs with estimated Azure costs.

``` text
TCO = ON-PREMISES vs. AZURE
```

------------------------------------------------------------------------

### 32. A --- Azure Cost Management

Azure Cost Management helps monitor, analyze, control, and optimize
cloud spending.

``` text
Pricing Calculator = ESTIMATE BEFORE
Cost Management    = TRACK / OPTIMIZE SPENDING
```

------------------------------------------------------------------------

### 33. D --- All of the Above

The Lesson 20 material identifies several factors that can affect Azure
costs, including:

-   Resource type
-   Region
-   Performance tier
-   Usage duration
-   Outbound data transfer

------------------------------------------------------------------------

### 34. B --- Service Level Agreement

An SLA describes Microsoft's availability commitment and associated
terms for an Azure service.

``` text
SLA = AVAILABILITY COMMITMENT
```

------------------------------------------------------------------------

### 35. A --- Service Credit

An eligible service may provide a service credit when Microsoft fails to
meet the applicable SLA terms and required conditions are satisfied.

------------------------------------------------------------------------

### 36. C --- Generally Available

A **Generally Available (GA)** service is fully released and is the
lifecycle stage the Lesson 20 material identifies for production use.

``` text
GA = GENERAL RELEASE / PRODUCTION-READY
```

------------------------------------------------------------------------

### 37. B --- Public Preview

Public Preview is broadly available for evaluation, but the Lesson 20
material distinguishes it from GA and cautions against treating preview
services as the default choice for critical production workloads.

------------------------------------------------------------------------

### 38. A --- Azure Reservation

Reservations can provide savings for eligible predictable workloads when
an organization makes a commitment.

``` text
Reservation = COMMIT + SAVE
```

------------------------------------------------------------------------

### 39. B --- Azure Spot Virtual Machine

Spot VMs use available unused compute capacity at a discount but can be
evicted when Azure needs the capacity.

``` text
Spot = DISCOUNTED + INTERRUPTIBLE
```

They are a better fit for workloads that can tolerate interruption.

------------------------------------------------------------------------

### 40. A and B

The key comparison is:

  Option            Best Memory
  ----------------- ------------------------------------------------
  **Reservation**   Predictable workload + commitment
  **Spot VM**       Discounted unused capacity + possible eviction

``` text
RESERVATION = COMMIT AND SAVE
SPOT        = SAVE BUT MAY BE EVICTED
```

------------------------------------------------------------------------

# 📊 Review Your Results

Count the questions you missed by lesson:

  Lesson   Area                      Questions     Missed
  -------- ------------------------- ----------- ----------
  **16**   Governance                1--8         \_\_\_\_
  **17**   Governance & Compliance   9--15        \_\_\_\_
  **18**   Security I                16--20       \_\_\_\_
  **19**   Security II               21--29       \_\_\_\_
  **20**   Pricing & Support         30--40       \_\_\_\_

Your weakest category should be the **first area you review**.

------------------------------------------------------------------------

# 🎯 What to Review

``` text
Missed 1–8
→ Review Lesson 16

Missed 9–15
→ Review Lesson 17

Missed 16–20
→ Review Lesson 18

Missed 21–29
→ Review Lesson 19

Missed 30–40
→ Review Lesson 20
```

------------------------------------------------------------------------

# 🏁 Final Check

Before moving on, make sure you can explain these without looking at
your notes:

``` text
Azure RBAC vs. Azure Policy
Policy Definition vs. Initiative vs. Assignment
CanNotDelete vs. ReadOnly Lock
Policy vs. Lock vs. Tag

Cloud Adoption Framework
Microsoft Purview
Trust Center
Azure Compliance Documentation
Sovereign Azure environments
DPA
Why Azure Blueprints is treated as legacy

Microsoft Defender for Cloud
Secure Score
Defense in Depth vs. Zero Trust
Verify Explicitly
Least Privilege
Assume Breach

NSG vs. Azure Firewall
Azure Firewall vs. DDoS Protection
Key Vault vs. Sentinel
Encryption vs. Secrets vs. Certificates
Dedicated Host
Identity Protection

Pricing Calculator vs. TCO Calculator
Cost Management
Factors affecting Azure costs
SLA and Service Credits
Preview vs. Generally Available
Reservation vs. Spot VM
```

If you can explain **why** each correct answer fits the
requirement---not just memorize the answer letter---you have a strong
grasp of Lessons 16--20.
