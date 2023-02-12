# Ubuntu RDP Server

## How To Use
+ Fork This Repo
+ Create a [ngrok account](https://dashboard.ngrok.com/) 
+ Get a [authtoken](https://dashboard.ngrok.com/get-started/your-authtoken) for free
+ Add a [Secret Variable](../../settings/secrets/actions/new) `NGROK_AUTH_TOKEN` and give your token there
+ Run [Github Action Workflow](../../actions/workflows/main.yml)
+ Go to [ngrok](https://dashboard.ngrok.com/tunnels/agents) to get hostname and port
+ If on windows connect using any RDP Client
+ If on linux open terminal and install xfreerdp and then copy & paste this:
```bash
xfreerdp /u:runner /p:toor  +clipboard /smart-sizing +offscreen-cache /f /v:<NGROK HostName>:PORT
```

## Credentials
Username: `runner`
Password: `toor`

