# Geocode-Conversion-Service

The Discrepancy Reporting web service is used by a reporting entity to initiate a Discrepancy Report. 

A discrepancy report contains the following:

| Name                                          | Condition                                                           | Description                                                                                            |
| --------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| resolutionUri                                 | MANDATORY                                                           | URI for responding entity to use for responses                                                         |
| reportType                                    | MANDATORY                                                           | Type of DR (enumeration)                                                                               |
| discrepancyReportSubmittalTimeStamp           | MANDATORY                                                           | Timestamp of Discrepancy Report Submittal                                                              |
| discrepancyReportId                           | MANDATORY                                                           | Unique (to reporting agency) ID of report                                                              |
| reportingAgencyName                           | MANDATORY                                                           | FQDN of the entity creating the report                                                                 |
| reportingAgentId                              | OPTIONAL                                                            | UserId of agent creating the report                                                                    |
| reportingContactJcard                         | MANDATORY                                                           | jCard of contact about this report                                                                     |
| problemService                                | Conditional, MUST be provided for specified DRs                     | Name of service or instance where discrepancy exists                                                   |
| problemSeverity                               | MANDATORY                                                           | A token representing the reporting entity’s opinion of the discrepancy’s severity |
| problemComments                               | Conditional, MUST be provided for specified DRs, OPTIONAL otherwise | Text comment                                                                                           |

## Owner

The owner of this repository approves all changes to the repository. 

This repository is owned by the NENA Core Services Committee, i3 Architecture working group.

#### Rules:

Specification Required. 

#### Contact:

[https://www.nena.org/page/911CoreSvcs](https://www.nena.org/page/911CoreSvcs) 

## Version History

### Discrepancy Reporting v 1.0

Version 1 OpenAPI schema for this service was originally defined in NENA-STA-010.3.2021. See https://www.nena.org/page/i3_Stage
