# Azure SQL Database
## SQL Database Service Tier Selection
During tier selection, we try to identify the amount of services we require while trying to balance the cost.

As of now, there are 4 tiers available:
1. Basic
2. Standard
3. Premium
4. Premium RS

A given tier supplies X amount of resources such as max. database size, max. storage elastic pool, max. databases per pool, backup retention.

Max. storage in an elastic pool is where you can combine multiple databases in a flexible resource pool. So resources of a database with low usage can be allocated to a database with high usage.

A given tier supplies Y amount of performance such as Max DTUs, Max concurrent workers, Max. concurrent logins, Max. concurrent sessions.

## Common Service Tier Use Cases

*Basic Service tier –*
- Small database
- Single active operation
- Ideal for development and testing

*Standard Service tier –*
- Support for multiple queries
- Low – medium IO requirements
- Ideal for cloud applications 
- Ideal for web applications

**If the application starts underperforming on the DB part then move up a tier.**

*Premium tier –*
- High transaction vol & high performance
- Supporting multiple users
- Ideal for mission-critical operations where uptime needs to be maximized

*Premium RS –*
- High transaction volume
- Used where highest availability is not critical
- Ideal for high-performance & analytical workloads

Because with analytical workloads, the thinking is that the sources of data can be reconstructed or re-accessed even if the data is lost as they are derived from other sources and fed into the data warehouse. We use Premium RS if we aren’t concerned about high availability but still want high performance.
