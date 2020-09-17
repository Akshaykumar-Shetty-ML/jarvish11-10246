### Keycloak Helm charts ###

  - **Add snappyflow helm chart repo**
	
	```
	$ helm repo add snappyflow https://snappyflow.github.io/helm-charts/
	"snappyflow" has been added to your repositories
	```
	
  - **Check repo added**
	```
	$ helm repo list
	NAME      		URL                                                            
	stable    		https://kubernetes-charts.storage.googleapis.com               
	snappyflow		https://snappyflow.github.io/helm-charts/
	```
  - **Update Helm repo**	
	```
	$ helm repo update
	```
	
	
  - **Get values.yaml content**	
	```
	$ helm inspect snappyflow/keycloak
	```
	
  - **Note: Below commands are applicable for Helm version 2. May not work for Helm version 3**

  - **Install with Default values**	
	```
	$ helm install snappyflow/keycloak --name my-app --namespace my-namespace
	```
	
  - **Get following parameters to pass to apm chart**

    ```
	  KEYCLOAKHOST  
	```
