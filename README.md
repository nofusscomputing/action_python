# No Fuss Computing - GH Action / Workflow for Python Projects

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
