# Tips and Tricks for everything not in Python.

## How to clone and push repository to GitHub with Token instead a username and password.

1. Generate a token in GitHub. Go to Settings -> Developer settings -> Personal access tokens -> Generate new token. Select the scopes you need and generate the token. Copy the token to the clipboard.
2. Clone the repository to your local machine. Open the terminal and type the following command:
```bash
git remote set-url origin https://<TOKEN>@github.com/<USERNAME>/<REPOSITORY>.git
```
3. Once you clone the repo that way you can push and pull the changes without the need to enter the username and password.