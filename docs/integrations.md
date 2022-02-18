This section provides an overview of Leapp's integrations, useful to extend the functionality of Leapp to 3rd party services.

An Integration contains all the information needed to connect to a 3rd party tool (e.g. AWS Single Sign-On) and *automatically* map access information into [Leapp Sessions](/sessions) in one time.


## Actions

Integrations have four main actions available: **Create**, **Delete**, **Sync**, and **Logout**.

| Action    | Description |
| --------- | ----------- |
| `CREATE`  | **Configure a new Integration with the data needed to start the authentication flow.** Required to Sync and map the service response into Sessions. |
| `DELETE`  | **Remove an existing Integration.** Also removes all the associated Sessions and wipes from the system everything related to it (Sessions, tokens, cache, etc.) |
| `SYNC`    | **Start the authentication flow to log into the Integration Provider.** Leapp will automatically retrieve all the related data and map the response into Sessions. Any change in your service of choice, require a manual Sync to reflect the current status. |
| `LOGOUT`  | **Disable the Integration.** Removes all the Sessions but keep the Integration data. Running a Sync will restore all Sessions tied to it. |

## Supported Services

| Service     | Supported |
| ----------- | --------- |
| AWS SSO     | :fontawesome-solid-check: |
| Okta        | Coming Soon |
| OneLogin    | Coming Soon |
| AzureAD     | Coming Soon |