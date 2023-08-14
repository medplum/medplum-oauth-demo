# Medplum OAuth Demo

This is a minimal demonstration of how to use Medplum as an OAuth2 Authorization Server.

It demonstrates:

- How to call the [/oauth2/authorize endpoint](https://medplum.com/docs/api/oauth/authorize) to initiate the authorization flow
- How to call the [/oauth2/token endpoint](https://medplum.com/docs/api/oauth/token) to exchange a code for an access token
- How to call the [/oauth2/userinfo endpoint](https://medplum.com/docs/api/oauth/userinfo) to retrive the current user details
- How to call the Medplum FHIR API with the access token

## Setup

Setup your account:

- [Register for a Medplum account](https://medplum.com/docs/tutorials/app/register)
- Create a `ClientApplication`
- Set the "Redirect URI" to "http://localhost:8000/"

Now you can run this demo using your HTTP server of choice. For example, using Python's built-in server:

```bash
python -m http.server 8000
```

Or using npm `http-server`:

```bash
npx http-server ./ -p 8000 -c-1
```

Open your web browser to <http://localhost:8000/>
