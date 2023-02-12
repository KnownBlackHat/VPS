# Linux RDP Server

## How To Use
+ Fork This Repo
+ Create a [ngrok account](https://dashboard.ngrok.com/) 
+ Get a [authtoken](https://dashboard.ngrok.com/get-started/your-authtoken) for free
+ Add a [Secret Variable](../../settings/secrets/actions/new) `NGROK_AUTH_TOKEN` and give your token there
+ Run [Github Action Workflow](../../actions/workflows/main.yml)
+ Go to [NGROK](https://dashboard.ngrok.com/tunnels/agents) to get url
+ If on windows connect using any RDP Client
+ If on linux open terminal and install xfreerdp and then copy & paste this:
```bash
xfreerdp /u:runner /p:toor /v:<NGROK URL>:PORT +clipboard /smart-sizing +offscreen-cache 
```

## Credentials
Username: `runner`
Password: `toor`
