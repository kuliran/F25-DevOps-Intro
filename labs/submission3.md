### GitHub Actions
A CI/CD tool that allows to create **workflows** perform automatic actions on specified events.

### Workflows
- Workflows are created under the `.github/workflows` directory and can have any names, but `.yaml`/`.yml` extension is mandatory.
- When an event occurs, all jobs hooked to it start running in a **cloud machine** provided by GitHub, performing the commands listed in the workflow configuration file.

### Workflow configuration
Referring to the [quickstart](https://docs.github.com/en/actions/get-started/quickstart), configurations have the following structure:
- name
- **event** on which the workflow is triggered (`on: [...]`)
- list of jobs, comprised of name, the **image** that the cloud machine will run (a virtual machine) and the **steps** (Linux commands to execute in order)