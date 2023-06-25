# 📄 The File CRM

The File CRM is a simple contact management app that allows you to keep full control of your data.

## Features

Your data will be structured like this:

```bash
data/
  project1/
    config.json // contains the project configuration
    contacts/
      contact1.md // contains the contact data
      contact2.md // contains the contact data
    ...
  project2/
    config.json
    contacts/
      contact1.md
      contact2.md
    ...
  ...

```

- You can manage *multiple* CRM **projects**.
- Every project is a folder of files on your local machine.
- Every project has a **pipeline** of stages configured, e.g. "Lead", "Contacted", "Customer", "Lost".
- For every **contact** in the project, a Markdown file is created in the project folder.

## Prerequisites

You'll need Docker and docker-compose installed on your machine.

## Setup & Running the App

First, clone this repository:

```bash
git clone https://github.com/kadrian/thefilecrm-backend.git
cd thefilecrm-backend
```

Then, run the following command to start the backend:

```bash
docker-compose up
```

The backend will listen on `localhost:3333` by default. It will use the `./data` folder from this repository (see the files above).

## Connect the frontend to your backend 
- Go to [thefilecrm.com](https://thefilecrm.com).
- The frontend should already connect to your backend on `localhost`.
- Start working on your local data.

## Troubleshooting
If you're having trouble connecting to `localhost` from another origin, try the following:

### Brave Browser
Add `@@||localhost^$domain=thefilecrm.com` into [brave://adblock](brave://adblock)`
[source](https://community.brave.com/t/brave-blocks-localhost-needs-shields-off-to-have-functioning-website/260084/2)
