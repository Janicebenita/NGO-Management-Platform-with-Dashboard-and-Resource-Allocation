# NGO Project Operations Agent Explainability

## Decision and Reasoning Process

The agent's decision process begins by identifying the projects and operational question specified by the user. It reasons from available database fields, including project status, dates, thematic area, region, donor information, and resource records, and then presents observations or recommendations linked to those fields.

For timeline monitoring, the agent compares recorded start, end, and MOU-extension dates with the requested reporting period. For portfolio summaries, it groups or filters project records and clearly separates calculated findings from management recommendations.

## Inputs and Data Sources Used

The primary input data used by the agent comes from authenticated records stored by the Flask and MySQL NGO management platform. These data sources may include project names, ERP codes, project years, thematic areas, regional-office details, donor information, MOU dates, extensions, project status, and resource-allocation information.

User-selected search terms, filters, reporting periods, and requested export scope are also treated as inputs. The agent does not assume access to financial, beneficiary, donor, or impact information that is not present in the platform's records.

## Outputs and Supporting Evidence

The agent can produce project summaries, status observations, timeline alerts, missing-data notes, resource-planning suggestions, and report-ready information. Each output should identify the relevant project and the stored fields or dates that support the conclusion.

Excel exports and dashboard totals are summaries of the available records rather than independent verification of project performance. Users should compare significant findings with approved project documents, donor agreements, financial records, and field reports.

## Limits, Constraints, and Known Issues

A major limitation is that the agent is only as reliable as the information entered and maintained in the database. Missing updates, incorrect status values, incomplete MOU dates, or absent resource records can produce incomplete or misleading conclusions.

Another constraint is that the current platform is an educational management implementation and does not by itself verify impact, financial compliance, donor approval, safeguarding requirements, or field execution. Advanced analytics, role-based permissions, notifications, cloud deployment, document management, and PDF reporting are listed as future enhancements and must not be represented as completed capabilities.

## Uncertainty and Human Review

The agent reports uncertainty whenever records are missing, inconsistent, outdated, or insufficient for the requested decision. It avoids presenting inferred delays, shortages, or project outcomes as confirmed facts unless the supporting database fields are available.

Authorized program, finance, donor-management, and organizational personnel must review important outputs before action is taken. Human approval remains necessary for project creation, status changes, MOU extensions, resource allocation, funding decisions, and external reporting.

