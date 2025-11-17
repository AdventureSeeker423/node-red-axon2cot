<h1 align='center'>node-red-axon2cot</h1>

<p align='center'>A node red flow using an Axon API key to create COT messages to be sent to a TAK server.</p>

<p align='center'>Pulls both Axon Body and Axon Fleet details and locations.</p>

<p align='center'>Portions of this code are derived from https://github.com/dfpc-coe/etl-axon licensed under the MIT License.</p>

## Pre-Requisites / Setup

1. Contact the administrator of the Axon Evidence Account to create an API Token.
2. From the admin account navigate to the "Admin" tab![rtaImage](https://github.com/user-attachments/assets/050ba165-7483-4b27-89d3-734abe623d13)
3. Then select "API Settings" under "Security Settings"![image](https://github.com/user-attachments/assets/f83d665c-aea6-4077-8b2d-ea04105644f7)
4. Click "Create Client" & fill in a name - IE "TAK Server"
5. For API permissions select the following:
    - `Device: state.any.read Allowed`![rtaImage](https://github.com/user-attachments/assets/b3869554-9461-49b5-a5c7-a1915f799aeb)

    - `Response: self.locate: Allowed`
    - `Response: self.alert_mark: Allowed`
    - `Response: any.locate: Allowed`![rtaImage](https://github.com/user-attachments/assets/cb494eeb-f031-4fcc-95b0-a5afbc73596d)

    - `Users: read: Allowed`![rtaImage](https://github.com/user-attachments/assets/99584d98-f2ad-4a95-b0ce-fbd311d3c33b)

6. Create the client & Provide the:
- Secret
- Partner ID
- Client ID
- Agency Domain (<your-agency>.evidence.com)![rtaImage](https://github.com/user-attachments/assets/10316d45-6ec8-484d-8444-6d028bb1f9e9)

## Deployment
