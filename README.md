<span style="text-align: center;">

# No Fuss Computing - GH Action / Workflow for Python Projects

<br>

![Endpoint Badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnofusscomputing%2Faction_python%2Frefs%2Fheads%2Fdevelopment%2F.centurion%2Fproject_status.json)



----

<br>

![GitHub forks](https://img.shields.io/github/forks/nofusscomputing/action_python?logo=github&style=plastic&color=000000&labell=Forks) ![GitHub stars](https://img.shields.io/github/stars/nofusscomputing/action_python?color=000000&logo=github&style=plastic) ![Github Watchers](https://img.shields.io/github/watchers/nofusscomputing/action_python?color=000000&label=Watchers&logo=github&style=plastic)



<br>

This project is hosted on our [Gitea](https://nofusscomputing.com/git/actions/python) instance and has a read-only copy hosted on [Github](https://nofusscomputing.com/git/nofusscomputing/action_python)

----

**Stable Branch**

----

**Development Branch** 

----
<br>

</span>

links:

- [Issues](https://nofusscomputing.com/git/actions/python/issues)

- [Merge Requests (Pull Requests)](https://nofusscomputing.com/git/actions/python/pulls)


To use this workflow within your project add a file at path `.github/workflows/ci.yaml` or add the job to your existing CI file.


``` yaml

---

name: 'CI'

on:
  push:
    branches:
      - '**'
    tags:
      - '*'


jobs:


  python:
    name: 'Python'
    uses: nofusscomputing/action_python/.github/workflows/python.yaml@development
    secrets:
      WORKFLOW_TOKEN: ${{ secrets.WORKFLOW_TOKEN }}

```



## Contributing

All contributions for this project must be conducted from our [Gitea](https://nofusscomputing.com/git/pytest/simplified).

For further details on contributing please refer to the [contribution guide](CONTRIBUTING.md).


## Other

This repo is release under this [license](LICENSE)
