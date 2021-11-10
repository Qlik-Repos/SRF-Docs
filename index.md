# ReadMe

The SRF is the Qlik Sense Security Rules Framework.

### Components
#### [Roles](./docs/roles/ReadMe.md)
#### [Security Rules](./docs/SecurityRules/ReadMe.md)
#### [Custom Properties](./docs/CustomProperties/ReadMe.md)
### [Change Log](./docs/ChangeLog.md)

## About: SRF
### SRF Principles
- Consistency
  - Consistent approach to drive quality deliveries
  - Version control to align framework with product versions
- Automation
  - Maximise ROI
  - Remove manual errors
  - Support DevOps and automate DR
- Governance & Self-Service
  - Users are authorised for both functionality and content
  - Support collaboration and self-service publication
  - Control quality through rigour and assurance
- Operational Risks
  - Limiting the need to change Qlik platform
  - Lower learning curve for Operations to run the environment
  - Improve maintainability through logical separation of rules
  - design changes are exception based

### SRF Scope
- Authentication is Out of Scope of the SRF. However, the method of authentication will impact the both the syntax of the implemented rules and potential certain design components. 
- Row and Column level data security referred to as either Section Access or Dynamic Data Reduction. This is Out of Scope as this should/must be covered as part of the Data Content Strategy.
- Sheet authorisation is Out of Scope of the base framework. If identified as a mandatory requirement this would be considered as additional work to be covered during the project deliver. 

### SRF Artefacts
The SRF includes the following:
- Configuration File: source file of rules, streams, custom properties that can be imported into Qlik Sense via the Configuration Migrator. These rules have been designed to be scalable, flexible and are proven in many production sites. Importantly, through version control and product alignment this framework is designed to minimise the impact of product updates.
- Security Rules Framework: A knowledge artefact that provides details and knowledge artefacts
- [Unit Test Cases](./docs/RM-UnitTestCases.md): that are completed off-site and can be leveraged as inputs into acceptance testing

### Resource Authorisation
The SRF includes flexible Authorisation Models. The authorisation applied is controlled via Custom Properties. This reduces/removes the need and associated risk of creation, updating and deleting rules directly. It is anticipated that certain edge cases may need modifications to these base rules. 

A resource specifically refers to: Analtyics Connections, Apps, Content Libraries, Data Connections, Extensions and Streams . The custom property, `@groupswithaccess`, controls which user groups can read the resource.
-	Null or Not Defined: the resource is not available to general users. It is available to site administrators such as Content Admins.
-	When defined the value of the custom property is compared to the user. If the comparison results in True, the resource is available. It is suggested that if a resource should be available to all users then a specific group is established that includes all users. I.e. Qlik_Access.


