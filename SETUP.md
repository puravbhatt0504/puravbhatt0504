# Profile Views Counter Setup

The Profile Views badge uses GitHub's repository traffic API.
 To make it work, add a **Personal Access Token** as a secret:

## 1. Create a Personal Access Token (PAT)

1. Go to **GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)**
2. Click **Generate new token (classic)**
3. Give it a name (e.g. `Profile Views Counter`)
4. Select the **`repo`** scope
5. Click **Generate token** and copy it

## 2. Add the token as a repository secret

1. Go to your profile repo: **github.com/puravbhatt0504/puravbhatt0504**
2. Click **Settings → Secrets and variables → Actions**
3. Click **New repository secret**
4. Name: `TRAFFIC_TOKEN`
5. Value: paste the token you copied
6. Click **Add secret**

## 3. Trigger the workflow

Go to **Actions** → **GitHub Snake Game** → **Run workflow**. After it completes, the Profile Views badge will show real view counts from your profile repository's traffic data.
