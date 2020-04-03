# setup notes

## openstack (i.e. the NCI cloud)

- probs easiest thing to do is install the python
  [openstackclient](https://docs.openstack.org/python-openstackclient/latest/)
  CLI tool (I used [pipx](https://github.com/pipxproject/pipx/))
  
- then, create a `~/.config/openstack/clouds.yaml` file which contains your NCI
  access info, e.g.
  
```YAML
clouds:
  nci:
    auth:
      auth_url: https://cloud.nci.org.au:5000
      project_name: rw17
      username: <NCI_USERNAME>
      password: <NCI_PASSWORD>
```
