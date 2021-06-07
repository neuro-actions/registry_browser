# An action to start Filebrowser

This action launches an instance of [Docker Registry Frontend](https://github.com/neuro-inc/docker-registry-frontend) and opens it in the default browser.

Has no required arguments.

### Quick example

```
jobs:
  browser:
    action: gh:neuro-actions/registry_browser@v1.0.0
```

## Arguments

### `job_name`

Predictable subdomain name which replaces the job's ID in the full job URI. `""` by default.

### Example

```
args:
	job_name: "filebrowser-job"
```

### `http_auth`

Whether to use HTTP authentication for the Filebrowser instance. `"True"` by default.

### Example

```
args: 
	http_auth: "False"
```