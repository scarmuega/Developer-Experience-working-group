# Well-Architected Framework

## Rationale

Cloud-development platforms usually provide a "well-architected framework" that describes their view of how to approach the development of complex systems on top of their platforms.

Here are some examples:

AWS: https://aws.amazon.com/architecture/well-architected
Azure: https://learn.microsoft.com/en-us/azure/architecture/framework/

In essence, each framework provides a set of best-practices on how to approach different development disciplines, such as: security, reliability, performance-optimization, monitoring, tracing, etc.

Having a "Cardano Well-Architected Framework" in a similar fashion to the mentioned above would serve as useful guidelines for developer teams entering the ecosystem.

## Roadmap / Status

- [ ] Define scope for v1
- [ ] Prepare draft document
- [ ] Identify KOLs for each topic
- [ ] Gather content from KOLs
- [ ] Gather feedback
- [ ] Publish v1

> KOL: A key opinion leader (KOL) is an individual who is widely recognized as an authority or expert in a specific field or industry.

## How to contribute
- By submitting a PR with changes to the scope (table of contents)
- By creating a new .md file that includes relevant information on any of the specific topics (it can be references to outside material or original content)
- By proposing candidate KOLs that would pontentially be able to fullfil the content for any of the topics.

## Maintenance of this Framework
- How will we keep this framework up to date over time?
- Define ownership and responsibilities

## Versioning
- What is our plan for breaking changes? (ie major upgrades to Plutus)
- When will the need for discrete versions to be acknowledged?
- Perhaps versioning can be within the scope of **Best Practices** in each Discipline?

## Scope

The following is a _live_ list of topics that the Well-Architected framework for Cardano should include. It's organized by broad disciplines that are involved in the process of building a dApp.

1. Reliability
2. Security
3. Cost Optimization
4. Performance
5. Decentralisation
6. Scalability
7. UX/UI
8. Documentation
9. Maintainability
10. Testing / Tooling

> Note: #8 + #9 could be combined, just as #10 could be split in two. We will adjust this list of Disciplines as needed as we add details to the outline.

Each discipline describes relevant _principles_ and _best practices_. _Reference Implementations_ and _Further Reading / Related Articles_ are provided so that developers can learn from research and by example about how to apply principles and best practices.

> **Principle**: a fundamental rule or guideline that should be followed when designing and building software applications. Principles are typically broad, general statements that provide guidance and direction for software development.

> **Best Practice**: a specific approach or technique that has been shown to be effective in solving a particular problem or achieving a specific goal in software development. Best practices are typically based on the experiences and expertise of experts in the field, and they provide guidance on how to design and implement software in a way that is maintainable, scalable, and extensible.

> **Reference Implementations**: a set of examples to illustrate Principles and Best Practices. Reference Implementations may include live projects, specific architectures, or topologies for decentralised applications.

> **Related Articles**: for example, common links, research, common exploits

> Introduction to each Discipline: What are key things people will have to consider during dapp development?

### Reliability
Reliability refers to the ability of a system to consistently provide access to data and services, regardless of hardware / software failures and excessive load. Reliability implies responsiveness, consistency and correctness of the data and processes of the system. The end-goal is to provide users with access to the resources they need, whenever they need them, without interruption.

Development teams should be aware of how to develop Cardano applications that avoid common SPOs (single point of failure) and implement fallback mechanisms by taking into account principles such as automation and observability early on, during the design phase of their projects.

#### Principles
- Design for business requirements
- Design for failure
- Observability
- Automation
- Self-healing

#### Best Practices
- Permanent Failure Handling
- Transient Failure Handling
- Congestion Handling
- Rollback Handling
- Tx Retry Policies
- Traffic Load Balancing

#### Reference Implementations
2-3 sentence introduction highlighting some key decisions dev teams will need to make - Santiago


### Security

#### Principles
- Identity Management
- Infrastructure Security
- Application Security
- Contract Security
- Contract Auditing
- Property-based Testing

#### Best Practices
- Client-side Wallet Integration
- Server-side Key Management
- Node Network Topology
- Plutus Testing Pipeline

#### Reference Implementations
2-3 sentence introduction highlighting some key decisions dev teams will need to make - Santiago

### Cost Optimization

#### Principles
- Cost Estimation
- Cost Models
- Cost Monitoring
- Capacity Planning

#### Best Practices
- Cardano Node Capacity Planning
- DB-Sync Capacity Planning
- Dynamic Scaling

#### Reference Implementations

### Performance
To determine the responsiveness, speed, scalability, and stability characteristics of the application under stress tests and aligning to production requirements. End-to-end performance throughput of any application should support anticipated peak production load, including network load. Tests should detect concurrency issues and functionality errors when under load.

These tests should be performed without overloading the Cardano blockchain. Developers should in their best knowledge, determine how many users the application can handle before performance is compromised. Developers should determine failure plans before causing failures and errors in addition to congestion of the network.


#### Principles
- Load Testing
- Stress Testing
- Process Profiling
- Plutus Cost Model

#### Best Practices
- Mempool Optimization
- Tx Chaining
- Plutus Script Optimization

#### Reference Implementations


### Decentralisation
2-3 sentence introduction highlighting some key decisions dev teams will need to make - Michele

#### Principles
- Robustness
- Censorship Resistance
- Open Source
- Shared ownership
- Independence

#### Best Practices
- Eject buttons
- Headless Dapps

#### Reference Implementations


### Scalability
Project architectures should be designed with scaling in mind, even when starting small. Development teams must be aware of the design challenges inherent in scaling applications on Cardano. This framework provides an overview of potential tradeoffs between Scalability and other disciplines, so that development teams can build for present and future use.

#### Principles
#### Best Practices
#### Reference Implementations

### User Experience UX/UI
User Experience covers the component architecture and UI Elements of a dApp, that ensure the smoothest experience possible. Whether it’s reading data of the blockchain, or submitting new data. The experience shouldn’t be any different from interacting with a regular WebApp.

#### Principles
#### Best Practices
#### Reference Implementations


### Documentation
#### Principles
#### Best Practices
#### Reference Implementations

### Maintainability
#### Principles
#### Best Practices
#### Reference Implementations

### Testing / Tooling
#### Principles
#### Best Practices
#### Reference Implementations
