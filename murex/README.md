[architecture](https://www.murex.com/en/solutions/technology/mx3-architecture)

# MX.3
MX.3 is a client/server application based on a three-tier architecture structure
- The application tier contains the presentation layer, business layer, orchestration layer, and grid layer.
- requires high memory, low latency, and high availability
- it can be run on VMs, and no PaaS services are supported for the application (e.g. serverless or container)
  - Hybrid models of deployment (hybrid cloud) for MX.3 are subject to technical review by the Murex team.

# presentation layer
- For added security, we recommend you use VDI running a desktop application to access the presentation layer.
  - you can also access it through a web interface.

list of functions
- Sales and trading
- Treasury
- Investment management
- Balance sheet management
- Funding
- Risk management
- Operations
- Finance
- Collateral

# business layer
engines
- Pricing engines
- Workflow engines
- Calculation engines
- Accounting engines
- Datamart engines
- XVA engines
- Limits engines
- Risk engines
- Collateral engines

# orchestration layer
orchestration layer services distribute calculations on business layer engines

list of unit
- Position server
- Limits server
- Market risk server
- Collateral server
- Market data server
- XVA server
- (Transaction) Processing server
- Simulation server
  - for analysis and prediction
  - e.g. risk evaluate on Tx
- Clearing orchestrator

# technical layer
the foundation of the platform

list of functions

- AuthN: SAML
- AuthR
- Caching: in-memory data grid, for critical calculation and aggregation
- Messaging
- Cluster management
  - k8s: Elastic compute for market risk and reporting
  - M.3 Grid of CPU/GPU: for exotic(非常规衍生品) pricing
- Aggregation
- Service registry
- Logging
- Monitoring: Open Telemetry
- Database
  - Support Oracle, SAP ASE, MS SQL, pg(EDB)
  - Domain: Financial db, Datamart DB


# Murex DevOps tools
application-level DevOps

