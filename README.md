# trigger-workflow-action
Github action to trigger another workflow.

This is not an official action.

The provided token needs to have permissions to start an action - the token which is automatically generated in Github Actions does not have this permission. You will need to use a Github App token or Personal Access token.

Example usage:
```yaml
    - name: Trigger My Workflow
      uses: jackjoynson/trigger-workflow-action@v1
      with:
        workflow: build.yaml
        token: ${{ secrets.ACTION_TOKEN }}
        repository: example/repository
```

See [action.yaml](./action.yaml) for the full list of inputs.
