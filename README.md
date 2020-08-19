<h1 align="center">
 Deploy app to Google App Engine :rocket:
</h1>

<p align="center">This action allowed you publish application to <a href="https://cloud.google.com/appengine/">Google App Engine</a></p>

## :ticket: Inputs

### `service-account`

**Required** The service account private key (JSON), you can know how to create one [here](https://cloud.google.com/iam/docs/creating-managing-service-account-keys).


### `project-id`

**Required** The project-id in service account.

### `debug`

To test. Default `false`. PS: If true does not deploy

## :clipboard: Example usage

```yaml
- name: Deploy to Google App Engine
  uses: etereo-io/deploy-gae-action
  with:
    service_account:  ${{ secrets.SERVICE_ACCOUNT }}
    project_id: ${{ secrets.PROJECT_ID }}
    gae_config_path: './app.yaml'

```

## :memo: License

This project is under license from MIT. See the [LICENSE](/LICENSE) file for more details.