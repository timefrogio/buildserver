### README

The repository contains a self-hosted linux agent image for Azure Pipelines and a simple azure pipeline definition to push the agent image to an Azure Container Registry. Following the instructions below will build the initial agent image and push it to your container registry to the location you specify using a variable library.

---

### INSTALL

1. Clone this repository to an Azure DevOps project in your organization

2. Create a Kubernetes service connection in your Azure DevOps project

3. Create a variable library in Azure DevOps Pipelines with the following variables defined

   | Variable Name                 | Example Value      |
   | ----------------------------- | ------------------ |
   | repository                    | myrepo/buildserver |
   | container-registry            | myrepo.azurecr.io  |
   | custom-build-server-start-tag | 1.0.0              |

 4. Create a new Azure DevOps build pipeline using the `azure-pipeline.yaml` file

 5. Run the pipeline

---

### RUN

Please refer to the instructions [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops#start-the-image-1) for guidance on how to run this image.

---

### CONTACT

[timefrog@timefrog.io](mailto://timefrog@timefrog.io)
[@timefrogio](https://twitter.com/timefrogio)