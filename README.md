# Django Web Application
- Description: Social Net + Project Post Web Aplication

## Features
- User authentication (Login/Register/Logout)
- Automatic sendings Email confirmation / Password recovery
- Search bar (by developer name or project title)
- Private messaging
- Vote system (Positiv or Negative) + Feedback by Project
- Admin panel
- User Profile View for other users with all social links and projects

# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
make clean install test
```

Check for devsearchantonio in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/devsearchantonio`
- Then populate it:

```bash
##   e.g. if group is "{group}" and project_name is "devsearchantonio"
git remote add origin git@github.com:{group}/devsearchantonio.git
git push -u origin master
git push -u origin --tags
```

Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
devsearchantonio-run
```

# Install

Go to `https://github.com/{group}/devsearchantonio` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:

```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:

```bash
git clone git@github.com:{group}/devsearchantonio.git
cd devsearchantonio
pip install -r requirements.txt
make clean install test                # install and test
```
Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
devsearchantonio-run
```
