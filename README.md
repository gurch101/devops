# Devops

A bunch of ansible playbooks to provision and configure digital ocean droplets

### Installation

1. `pip install -r requirements.txt`

2. add your DigitalOcean API key as an environment variable:

    ```
    export DO_API_KEY=<your API key here>
    ```

3. add an [SSH Key](https://cloud.digitalocean.com/settings/security)

4. run `python digital_ocean.py --ssh-keys` to get your ssh key id

5. setup `instances.yml` with your droplet details

6. add a password in `group_vars/all` for a ssh user

7. run `ansible-playbook provision.yml` to create your droplets!
