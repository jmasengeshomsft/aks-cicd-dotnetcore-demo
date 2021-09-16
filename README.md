# aks-cicd-dotnetcore-demo


variables:
  - name: solution
    value: '**/*.sln'
  - name: buildPlatform
    value: 'Any CPU'
  - name: buildConfiguration
    value: "Release"
  - name : NugetSecurityAnalysisWarningLevel
    value : none
  - name: imageName
    value : <acr image name/repository>
  - name: azureSubscriptionEndpoint
    value : <azure subscription service connection>
  - name: azureContainerRegistry
    value: <acr instance url>
  - name: azureResourceGroup
    value: <aks cluster resource group>
  - name : kubernetesCluster
    value: <aks cluster name>
  - name: namespace
    value: <pod namespace, must be created before running pipeline>
  - name: useClusterAdmin
    value: <set to true if using the user access key as password>
  - name: acr_connection
    value: <acr service connection with push/pull>
