# Devops

A bunch of ansible playbooks to provision and configure digital ocean droplets

### Installation

1. `pip install -r requirements.txt`

2. add your DigitalOcean API key as an environment variable:

    ```
    export DO_API_KEY=<your API key here>
    ```

3. setup `instances.yml` with your droplet details. See `provisioners/digitalocean.yml` for variables.

4. Add `deploy_user_passwd` to `instances.yml`. This is used to create a user on new nodes and can be set to any encrypted password.

5. run `ansible-playbook webservers.yml` to create your droplets!
