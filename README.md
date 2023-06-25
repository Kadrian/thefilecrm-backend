# The File CRM

The File CRM is a simple contact management app that allows you to keep full control of your data.

## Features

The data is structured as follows:

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

Then, run the following command to start the app:

```bash
docker-compose up
```

By default, that will use the `./data` folder and run a server on [localhost:3000](http://localhost:3000).

Then you can go to [thefilecrm.com](https://thefilecrm.com), connect the frontend app to your backend and start working on your local data.

