# Issues & Troubleshooting 

This document records the technical hurdles, CLI deployment errors, schema binding issues and runtime permission conflicts encountered during the deployment of the SAP BTP Incident Management scenario, along with their root causes and resolutions.

## Issue Summary

| Category | Observed Error | Root Cause | Technical Resolution |
| :--- | :--- | :--- | :--- |
| **Authentication & CLI** | `cf login` fails/targets incorrect subaccount | authentication tokens/regional endpoint mismatch | Executed `cf login -a <API_URL> --sso` with target org and space parameters |
| **Database Binding** | HDI container deployment fails with `403 Forbidden` / `Service broker error` | SAP HANA Cloud instance stopped or missing HDI service bindings | Verified database instance status in HANA Cloud Central; recreated HDI binding in `mta.yaml` |
| **App Building (MTA)** | `mbt build` fails during npm module compilation | Outdated local node modules or missing build tools inside BAS workspace | Cleared `node_modules`, executed `npm install` and updated `@sap/hdi-deploy` dependencies |
| **Work Zone Portal** | Application tile yields `404 Not Found` or `Access Denied` on launchpad | Unassigned Role Collections or un-fetched HTML5 Application Repository content | Executed **Fetch** on Content Provider inside Work Zone and mapped target Role Collection in BTP Cockpit |
