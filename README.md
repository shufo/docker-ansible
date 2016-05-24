# docker-ansible-alpine

Dockerized ansible on Alpine.

## Usage

- Use inventory file

```
docker run -it -v $(pwd)/hosts:/hosts shufo/ansible -i /hosts all -m ping
```

- Use `ansible-playbook`

```
docker run -it -v $(pwd)/hosts:/hosts --entrypoint=ansible-playbook shufo/ansible playbook.yml
```
