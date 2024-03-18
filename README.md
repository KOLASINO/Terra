# Terraform
Terraform is an open-source infrastructure as a code tool created by Hashicorp, it allows users to define and manage cloud and on-premises resources in human-readable configuration files. Most users prefer Terraform because of its ability to work with various providers such as Azure, AWS, and GCP, to automate changes, track infrastructure, and collaborate with teams.

Terraform in Azure: To use Terraform in Azure, you need to authenticate to Azure using one of the following methods:

Azure CLI: To authenticate, run the az login command and follow the prompts.

Service Principal: To authenticate using a service principal, you need to create a service principal and assign it the appropriate permissions. (az login --service-principal -u "CLIENT_ID" -p "CERTIFICATE_PEM" --tenant "TENANT_ID")

I prefer to use the Visual Studio Terraform extension to work with Terraform from within the VS IDE. However, you can also use Azure Cloud Shell and Eclipse. Once you start deploying Azure resources using Terraform, It is advisable to stick with using Terraform for future deployments for consistency.

Hashicorp made Terraform quite easy to understand and use because you can find samples of how to deploy Azure resources on their website https://lnkd.in/dbQTEy4U so you don't have to cram commands. Terraform has several commands that can be used to manage your infrastructure but the major ones are terraform.Init, terraform.plan, terraform.apply, and terraform.destroy.

✅ init: Prepare your working directory for other commands.
✅validate: Check whether the configuration is valid.
✅plan: Show changes required by the current configuration.
✅apply: Create or update infrastructure.
✅destroy: Destroy previously-created infrastructure.
✅fmt: Reformat your configuration in the standard style.
✅get: Install or upgrade remote Terraform modules.
✅import: Associate existing infrastructure with a Terraform resource.
✅output: Show output values from your root module.
✅providers: Show the providers required for this configuration.
✅refresh: Update the state to match remote systems.
✅show: Show the current state or a saved plan state.
✅taint: Mark a resource instance as not fully functional.
✅untaint: Remove the ‘tainted’ state from a resource instance.
✅version: Show the current Terraform version.
✅workspace: Workspace management.

The attached screenshots illustrate how to create a Virtual machine in Azure using Terraform. In Terraform, it is a common practice to create files using the .tf extension. In VS code, Terraform reads all the .tf files in the directory as one file, so creating separate files like (main.tf, provider.tf, variables.tf) makes the environment easy to read and understand by others.

In the VS environment, Terraform automatically creates the following folder as seen on the left pane of the screenshot.
✅ terraform. lock. hcl
✅ terraform.tfstate
✅ terraform.tfstate.backup
![image](https://github.com/KOLASINO/Terra/assets/135536416/f3cf0bfb-9e20-40b2-86cd-0e07914ff73d)
![image](https://github.com/KOLASINO/Terra/assets/135536416/9af2b79d-da2c-4e6b-846c-26921528356d)
![image](https://github.com/KOLASINO/Terra/assets/135536416/013c8fbf-0180-4f72-a7c2-06ea1cc49102)
![image](https://github.com/KOLASINO/Terra/assets/135536416/06016906-107a-4b23-a83e-225d75d3d971)



