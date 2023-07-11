# Comparing `tmp/devopipe-0.1.4.tar.gz` & `tmp/devopipe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopipe-0.1.4.tar", max compression
+gzip compressed data, was "devopipe-0.1.5.tar", max compression
```

## Comparing `devopipe-0.1.4.tar` & `devopipe-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2023-07-11 20:05:07.000304 devopipe-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-11 20:05:07.000304 devopipe-0.1.4/devopipe/__init__.py
--rwxr-xr-x   0        0        0      503 2023-07-11 20:01:49.410687 devopipe-0.1.4/devopipe/src/downloaded_template.yaml
--rwxr-xr-x   0        0        0    17457 2023-07-11 20:03:36.962023 devopipe-0.1.4/devopipe/src/main.py
--rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.4/devopipe/src/setup_template.yaml
--rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.4/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
--rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.4/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
--rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.4/devopipe/src/templates/IaC/aws/blueprints.tf
--rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.4/devopipe/src/templates/IaC/aws/create-namespace.yaml
--rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.4/devopipe/src/templates/IaC/aws/create-vcluster.yaml
--rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.4/devopipe/src/templates/IaC/aws/developer-role.tf
--rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.4/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
--rwxr-xr-x   0        0        0     1818 2023-07-08 07:27:31.748556 devopipe-0.1.4/devopipe/src/templates/IaC/aws/main.tf
--rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.4/devopipe/src/templates/IaC/aws/values/argocd.yaml
--rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.4/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
--rwxr-xr-x   0        0        0      191 2023-07-08 07:28:37.216100 devopipe-0.1.4/devopipe/src/templates/IaC/aws/variables.tf
--rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.4/devopipe/src/templates/IaC/aws/vpc-module.tf
--rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.4/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
--rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.4/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
--rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.4/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
--rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.4/devopipe/src/templates/ci-pipeline/get-artifact.yaml
--rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.4/devopipe/src/templates/ci-pipeline/set-artifact.yaml
--rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/deployment.yaml
--rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
--rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
--rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
--rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
--rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.4/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
--rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.4/devopipe/src/templates/kubernetes/aws/service-account.yaml
--rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.4/devopipe/src/templates/kubernetes/aws/storage.yaml
--rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.4/devopipe/src/templates/tests/database-sonarqube.yaml
--rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.4/devopipe/src/templates/tests/deployment-sonarqube.yaml
--rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.4/devopipe/src/templates/tests/storage_sonarqube.yaml
--rw-r--r--   0        0        0      486 2023-07-11 20:05:08.840304 devopipe-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-11 21:36:42.178982 devopipe-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 21:36:42.178982 devopipe-0.1.5/devopipe/__init__.py
+-rwxr-xr-x   0        0        0      503 2023-07-11 20:01:49.410687 devopipe-0.1.5/devopipe/src/downloaded_template.yaml
+-rwxr-xr-x   0        0        0    19388 2023-07-11 21:33:34.471235 devopipe-0.1.5/devopipe/src/main.py
+-rwxr-xr-x   0        0        0      503 2023-05-20 15:55:35.377136 devopipe-0.1.5/devopipe/src/setup_template.yaml
+-rwxr-xr-x   0        0        0      682 2023-06-03 15:07:59.926738 devopipe-0.1.5/devopipe/src/templates/IaC/aws/argocd/argocd.yaml
+-rwxr-xr-x   0        0        0      431 2023-06-03 15:06:38.526922 devopipe-0.1.5/devopipe/src/templates/IaC/aws/argocd/git-repo-secret.yaml
+-rwxr-xr-x   0        0        0     1060 2023-06-03 12:26:50.974002 devopipe-0.1.5/devopipe/src/templates/IaC/aws/blueprints.tf
+-rwxr-xr-x   0        0        0      193 2023-07-08 14:25:02.731315 devopipe-0.1.5/devopipe/src/templates/IaC/aws/create-namespace.yaml
+-rwxr-xr-x   0        0        0      446 2023-07-08 14:24:50.460031 devopipe-0.1.5/devopipe/src/templates/IaC/aws/create-vcluster.yaml
+-rwxr-xr-x   0        0        0     2900 2023-05-31 16:31:15.386462 devopipe-0.1.5/devopipe/src/templates/IaC/aws/developer-role.tf
+-rwxr-xr-x   0        0        0     2441 2023-07-08 07:51:10.532504 devopipe-0.1.5/devopipe/src/templates/IaC/aws/kubernetes-addons.tf
+-rwxr-xr-x   0        0        0     1818 2023-07-08 07:27:31.748556 devopipe-0.1.5/devopipe/src/templates/IaC/aws/main.tf
+-rwxr-xr-x   0        0        0       86 2023-05-31 16:32:54.171449 devopipe-0.1.5/devopipe/src/templates/IaC/aws/values/argocd.yaml
+-rwxr-xr-x   0        0        0     2773 2023-07-08 17:09:20.058014 devopipe-0.1.5/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml
+-rwxr-xr-x   0        0        0      191 2023-07-08 07:28:37.216100 devopipe-0.1.5/devopipe/src/templates/IaC/aws/variables.tf
+-rwxr-xr-x   0        0        0      702 2023-05-31 16:31:15.397464 devopipe-0.1.5/devopipe/src/templates/IaC/aws/vpc-module.tf
+-rwxr-xr-x   0        0        0     1059 2023-07-07 19:50:26.479466 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml
+-rwxr-xr-x   0        0        0      926 2023-07-07 19:15:44.377038 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml
+-rwxr-xr-x   0        0        0     1206 2023-07-07 19:43:38.910184 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml
+-rwxr-xr-x   0        0        0      537 2023-07-07 19:50:37.893453 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/get-artifact.yaml
+-rwxr-xr-x   0        0        0      570 2023-07-07 19:47:05.401736 devopipe-0.1.5/devopipe/src/templates/ci-pipeline/set-artifact.yaml
+-rwxr-xr-x   0        0        0     1030 2023-05-29 06:15:10.217363 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment.yaml
+-rwxr-xr-x   0        0        0     1855 2023-05-29 06:14:47.653941 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml
+-rwxr-xr-x   0        0        0     1261 2023-06-02 14:50:54.153883 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_database.yaml
+-rwxr-xr-x   0        0        0     1093 2023-05-29 06:16:25.169533 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml
+-rwxr-xr-x   0        0        0      157 2023-05-29 06:16:31.583979 devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/pgadmin-secret.yaml
+-rwxr-xr-x   0        0        0     1552 2023-07-08 15:20:41.141561 devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml
+-rwxr-xr-x   0        0        0      227 2023-05-14 16:03:18.827923 devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/service-account.yaml
+-rwxr-xr-x   0        0        0      413 2023-05-30 21:28:15.835610 devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/storage.yaml
+-rwxr-xr-x   0        0        0     1270 2023-06-02 14:53:53.987792 devopipe-0.1.5/devopipe/src/templates/tests/database-sonarqube.yaml
+-rwxr-xr-x   0        0        0     1480 2023-06-02 20:45:12.895069 devopipe-0.1.5/devopipe/src/templates/tests/deployment-sonarqube.yaml
+-rwxr-xr-x   0        0        0      451 2023-06-02 16:35:55.368830 devopipe-0.1.5/devopipe/src/templates/tests/storage_sonarqube.yaml
+-rw-r--r--   0        0        0      486 2023-07-11 21:36:44.118982 devopipe-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 devopipe-0.1.5/PKG-INFO
```

### Comparing `devopipe-0.1.4/devopipe/src/main.py` & `devopipe-0.1.5/devopipe/src/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,42 +88,43 @@
         source_control = yaml_values["init"]["source_control"]
         database = yaml_values["init"]["database"]
         cd_tool = yaml_values["init"]["cd_tool"]
         monitoring_stack = yaml_values["init"]["monitoring_stack"]
 
 
     else:
-        #Give me: name of frontend, backend, databse, flyway image on docker compose,
-        # What type of migration tool are you using
-        typer.echo("What CI will you use?")
-        ci_system = choose_option(["Azure Pipelines", "GitHub Actions"]) # For Pipeline
-        typer.echo("What tests plataform will you use?")
-        tests = choose_option(["Sonarqube", "Codacy"]) # For Kubernetes or Pipeline
-        typer.echo("What service provider will you use?")
-        service_provider = choose_option(["On-prem", "AWS", "Azure", "GCP"]) # For Kubernetes and Terraform
-        region = typer.prompt("Wich cloud region do you wanna use? ")
-        ############num_environments = int(typer.prompt("How many environments will you have? ")) # For kubernetes and Terraform
-        environment_names = typer.prompt("What are the names of your environments (separated by commas)? ") # For kubernetes and Terraform
-        registry = choose_option(["ECR (Elastic Container Registry)", "ACR (Azure Container Registry)", "Docker Hub"]) # For Pipeline and Kubernetes
-        typer.echo("Your repositories are:")
-        repository_type = choose_option(["Public", "Private"]) # For Pipeline and Terraform 
-        typer.echo("What migration tool will you use?")
-        monitoring_stack = choose_option(["Flyway", "Liquibase"]) # For Terraform
-        typer.echo("What stack do you wanna use for monitorization?")
-        #Ask for Argocd
-        # Bitbucket or github
-        typer.echo("What Source Control will you use?")
-        source_control = choose_option(["Bitbucket", "GitHub"]) # For Source Control
-        # Qual base de dados
-        typer.echo("What Database will you use?")
-        database = choose_option(["Postgres"]) # For Source Control
-        typer.echo("Which Delievery tool will you use?")
-        cd_tool = choose_option(["Argocd"]) # For Source Control
-        typer.echo("Which Monitoring Stack will you use?")
-        monitoring_stack = choose_option(["ELK", "Prometheus + Loki"]) # For Terraform
+        print("else")
+        ###########Give me: name of frontend, backend, databse, flyway image on docker compose,
+        ########### What type of migration tool are you using
+        ##########typer.echo("What CI will you use?")
+        ##########ci_system = choose_option(["Azure Pipelines", "GitHub Actions"]) # For Pipeline
+        ##########typer.echo("What tests plataform will you use?")
+        ##########tests = choose_option(["Sonarqube", "Codacy"]) # For Kubernetes or Pipeline
+        ##########typer.echo("What service provider will you use?")
+        ##########service_provider = choose_option(["On-prem", "AWS", "Azure", "GCP"]) # For Kubernetes and Terraform
+        ##########region = typer.prompt("Wich cloud region do you wanna use? ")
+        ######################num_environments = int(typer.prompt("How many environments will you have? ")) # For kubernetes and Terraform
+        ##########environment_names = typer.prompt("What are the names of your environments (separated by commas)? ") # For kubernetes and Terraform
+        ##########registry = choose_option(["ECR (Elastic Container Registry)", "ACR (Azure Container Registry)", "Docker Hub"]) # For Pipeline and Kubernetes
+        ##########typer.echo("Your repositories are:")
+        ##########repository_type = choose_option(["Public", "Private"]) # For Pipeline and Terraform 
+        ##########typer.echo("What migration tool will you use?")
+        ##########monitoring_stack = choose_option(["Flyway", "Liquibase"]) # For Terraform
+        ##########typer.echo("What stack do you wanna use for monitorization?")
+        ###########Ask for Argocd
+        ########### Bitbucket or github
+        ##########typer.echo("What Source Control will you use?")
+        ##########source_control = choose_option(["Bitbucket", "GitHub"]) # For Source Control
+        ########### Qual base de dados
+        ##########typer.echo("What Database will you use?")
+        ##########database = choose_option(["Postgres"]) # For Source Control
+        ##########typer.echo("Which Delievery tool will you use?")
+        ##########cd_tool = choose_option(["Argocd"]) # For Source Control
+        ##########typer.echo("Which Monitoring Stack will you use?")
+        ##########monitoring_stack = choose_option(["ELK", "Prometheus + Loki"]) # For Terraform
 
     ## Create a template object
     #template = Template(template_content)
 
     ## Define the parameters
     #params = {'name': 'John', 'day': 'Monday'}
 
@@ -146,17 +147,18 @@
     typer.echo(f"Data Migration Tool: {data_migration}")
     typer.echo(f"Source Control: {source_control}")
     typer.echo(f"Database: {database}")
     typer.echo(f"Continuous Delievery Tool: {cd_tool}")
     typer.echo(f"Monitorization: {monitoring_stack}")
 
     if ci_system == "Azure Pipelines":
-        pipeline_frontend = mountAzurePipelineFrontend(registry)
+        template_dir = ["templates","ci-pipeline"]
+        pipeline_frontend = mountAzurePipelineFrontend(registry, template_dir)
         typer.echo(type(pipeline_frontend))
-        pipeline_backend = mountAzurePipelineBackend(registry)
+        pipeline_backend = mountAzurePipelineBackend(registry, template_dir)
         #mountAzurePipeline(registry)
     folder_path = "./.azure-pipelines/"
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
 
     #pipeline_frontend = ruamel.yaml.safe_load(pipeline_frontend)
     #pipeline_backend = ruamel.yaml.safe_load(pipeline_backend)
@@ -165,217 +167,229 @@
     #pipeline_backend_formatted_yaml = yaml.dump(pipeline_backend)
     
     save_template(pipeline_frontend, folder_path + "pipeline_frontend.yaml")
     save_template(pipeline_backend, folder_path + "pipeline_backend.yaml")
 
     # mount Terraform, Kubernetes
     if service_provider == "AWS":
-        mountTerraformAWS(name_cluster, environment_names, region)
-        mountKubernetesAWS(name_cluster, environment_names, region)
+        template_dir_terra = ["templates", "IaC", "aws"]
+        template_dir_kubernetes = ["templates", "kubernetes"]
+        template_dir_kubernetes_apps = ["templates", "kubernetes", "apps/"]
+        template_dir_kub_cloud = ["templates", "kubernetes", "aws/"]
+        mountTerraformAWS(name_cluster, environment_names, region, template_dir_terra)
+        mountKubernetesAWS(name_cluster, environment_names, region, template_dir_kubernetes, template_dir_kubernetes_apps, template_dir_kub_cloud)
 
 
     # mount CD tool
     if cd_tool == "Argocd":
-        mountArgoCD(environment_names)
+        template_dir_argocd = ["templates","IaC","aws", "argocd"]
+        mountArgoCD(environment_names, template_dir_argocd)
 
     # mount test tool
     if tests == "Sonarqube":
-        mountSonarqube(service_provider)
+        template_dir_sonarqube = ["templates", "tests"]
+        mountSonarqube(service_provider, template_dir_sonarqube)
 
 
 
-def mountSonarqube(service_provider):
+def mountSonarqube(service_provider, template_dir):
     if service_provider == "AWS":
         folder_path = "./kubernetes/aws/"
     
     if not os.path.exists(folder_path):
             os.makedirs(folder_path)
-    save_template(render_template("./src/templates/tests/database-sonarqube.yaml", {}), folder_path + "database-sonarqube.yaml")
-    save_template(render_template("./src/templates/tests/deployment-sonarqube.yaml", {}), folder_path + "deployment-sonarqube.yaml")
-    save_template(render_template("./src/templates/tests/storage_sonarqube.yaml", {}), folder_path + "storage_sonarqube.yaml")
+    save_template(render_template(template_dir, "database-sonarqube.yaml", {}), folder_path + "database-sonarqube.yaml")
+    save_template(render_template(template_dir, "deployment-sonarqube.yaml", {}), folder_path + "deployment-sonarqube.yaml")
+    save_template(render_template(template_dir, "storage_sonarqube.yaml", {}), folder_path + "storage_sonarqube.yaml")
 
 
 
-def mountArgoCD(environment_names):
+def mountArgoCD(environment_names, template_dir):
+    template_dir_vcluster_values = ["templates", "IaC", "aws", "values"]
     folder_path = "./IaC/"
     folder_path_argocd = folder_path + "argocd/"
     if not os.path.exists(folder_path_argocd):
         os.makedirs(folder_path_argocd)
 
-    save_template(render_template("./src/templates/IaC/aws/argocd/argocd.yaml", {}), folder_path_argocd + "argocd.yaml")
-    save_template(render_template("./src/templates/IaC/aws/argocd/git-repo-secret.yaml", {}), folder_path_argocd + "git-repo-secret.yaml")
+    save_template(render_template(template_dir, "argocd.yaml", {}), folder_path_argocd + "argocd.yaml")
+    save_template(render_template(template_dir, "git-repo-secret.yaml", {}), folder_path_argocd + "git-repo-secret.yaml")
 
     folder_path_values = folder_path + "values/"
     if not os.path.exists(folder_path_values):
         os.makedirs(folder_path_values)
     
-    save_template(render_template("./src/templates/IaC/aws/argocd/argocd.yaml", {}), folder_path_values + "argocd.yaml")
+    save_template(render_template(template_dir, "argocd.yaml", {}), folder_path_values + "argocd.yaml")
 
     for i, env_name in enumerate(environment_names):
-        save_template(render_template("./src/templates/IaC/aws/values/vcluster-config-init.yaml", {
+        save_template(render_template(template_dir_vcluster_values, "vcluster-config-init.yaml", {
             'url': "url_kubernetes",
             'username': "username",
             'password': "password",
             'argocd_name': env_name.lower() + "-apps",
             'argocd_path':  "environments/" + env_name.lower() + "/apps"
         }), folder_path_values + "vcluster-" + env_name.lower() + ".yaml")
 
 
 
-def mountKubernetesAWS(name_cluster, environment_names, region):
+def mountKubernetesAWS(name_cluster, environment_names, region, template_dir, template_dir_kubernetes_apps, template_dir_cloud):
     folder_path = "./kubernetes/"
     folder_path_aws = folder_path + "aws/"
     if not os.path.exists(folder_path_aws):
         os.makedirs(folder_path_aws)
 
     #mount Aws resources
-    save_template(render_template("./src/templates/kubernetes/aws/storage.yaml", {}), folder_path_aws + "storage.yaml")
-    save_template(render_template("./src/templates/kubernetes/aws/service-account.yaml", {}), folder_path_aws + "service-account.yaml")
+    save_template(render_template(template_dir_cloud, "storage.yaml", {}), folder_path_aws + "storage.yaml")
+    save_template(render_template(template_dir_cloud, "service-account.yaml", {}), folder_path_aws + "service-account.yaml")
 
     for i, env_name in enumerate(environment_names):
-        save_template(render_template("./src/templates/kubernetes/aws/ingress_aws.yaml", {
+        save_template(render_template(template_dir_cloud, "ingress_aws.yaml", {
             'frontend_service': 'myapp-x-default-x-' + env_name.lower() +'-vcluster',
             'backend_service': 'myapp-backend-x-default-x-' + env_name.lower() +'-vcluster',
             'frontend_route': '/frontend/',
             'backend_route': '/api/v1/',
         }), folder_path_aws + "ingress_aws" + env_name.lower() + ".yaml")
 
 
 
     #mount environment resources
     for i, env_name in enumerate(environment_names):
         folder_path_env = folder_path + env_name.lower() + '/apps/'
         if not os.path.exists(folder_path_env):
             os.makedirs(folder_path_env)
         
-        save_template(render_template("./src/templates/kubernetes/apps/deployment_backend.yaml", {}), folder_path_env + "/deployment_backend.yaml")
-        save_template(render_template("./src/templates/kubernetes/apps/deployment_database.yaml", {}), folder_path_env + "/deployment_database.yaml")
-        save_template(render_template("./src/templates/kubernetes/apps/deployment.yaml", {}), folder_path_env + "/deployment.yaml")
-        save_template(render_template("./src/templates/kubernetes/apps/pgadmin-deploy.yaml", {}), folder_path_env + "/pgadmin-deploy.yaml")
-        save_template(render_template("./src/templates/kubernetes/apps/pgadmin-secret.yaml", {}), folder_path_env + "/pgadmin-secret.yaml")
+        save_template(render_template(template_dir_kubernetes_apps, "deployment_backend.yaml", {}), folder_path_env + "/deployment_backend.yaml")
+        save_template(render_template(template_dir_kubernetes_apps, "deployment_database.yaml", {}), folder_path_env + "/deployment_database.yaml")
+        save_template(render_template(template_dir_kubernetes_apps, "deployment.yaml", {}), folder_path_env + "/deployment.yaml")
+        save_template(render_template(template_dir_kubernetes_apps, "pgadmin-deploy.yaml", {}), folder_path_env + "/pgadmin-deploy.yaml")
+        save_template(render_template(template_dir_kubernetes_apps, "pgadmin-secret.yaml", {}), folder_path_env + "/pgadmin-secret.yaml")
 
 
 
 
-def mountTerraformAWS(name_cluster, environment_names, region):
+def mountTerraformAWS(name_cluster, environment_names, region, template_dir):
     folder_path = "./IaC/"
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
 
-    rendered_template_variables = render_template("./src/templates/IaC/aws/variables.tf", {
+    rendered_template_variables = render_template(template_dir, "variables.tf", {
         'cluster_name': name_cluster,
         'state_region': region
     })
 
     rendered_template_namespaces = ""
     rendered_template_vclusters = ""
 
     for i, env_name in enumerate(environment_names):
         namespace_name = name_cluster.lower() + '-' + env_name.lower()
-        rendered_template_namespaces += render_template("./src/templates/IaC/aws/create-namespace.yaml", {
+        rendered_template_namespaces += render_template(template_dir, "create-namespace.yaml", {
             'namespace_name': namespace_name
         })
-        rendered_template_vclusters += render_template("./src/templates/IaC/aws/create-vcluster.yaml", {
+        rendered_template_vclusters += render_template(template_dir, "create-vcluster.yaml", {
             'vcluster_name': env_name.lower() + "-vcluster",
             'namespace_name': namespace_name,
             'values_file': "values/" + namespace_name + ".yaml",
             'depends_on': "kubernetes_namespace." + namespace_name
         })
 
     
     save_template(rendered_template_variables, folder_path + "variables.tf")
-    save_template(render_template("./src/templates/IaC/aws/vpc-module.tf", {}), folder_path + "vpc-module.tf")
-    save_template(render_template("./src/templates/IaC/aws/main.tf", {}), folder_path + "main.tf")
-    save_template(render_template("./src/templates/IaC/aws/kubernetes-addons.tf", {
+    save_template(render_template(template_dir, "vpc-module.tf", {}), folder_path + "vpc-module.tf")
+    save_template(render_template(template_dir, "main.tf", {}), folder_path + "main.tf")
+    save_template(render_template(template_dir, "kubernetes-addons.tf", {
         'create_namespace': rendered_template_namespaces,
         'create_vcluster': rendered_template_vclusters
     }), folder_path + "kubernetes-addons.tf")
-    save_template(render_template("./src/templates/IaC/aws/developer-role.tf", {}), folder_path + "developer-role.tf")
-    save_template(render_template("./src/templates/IaC/aws/blueprints.tf", {}), folder_path + "blueprints.tf")
+    save_template(render_template(template_dir, "developer-role.tf", {}), folder_path + "developer-role.tf")
+    save_template(render_template(template_dir, "blueprints.tf", {}), folder_path + "blueprints.tf")
 
 
 
 
 
-def mountAzurePipelineFrontend(registry):
-    phases_frontend = mountAzurePipeline(registry, 'frontend_image', 'frontend_artifact', ['AWS_FRONTEND_REPOSITORY', 'frontend_react'] )
+def mountAzurePipelineFrontend(registry, template_dir):
+    phases_frontend = mountAzurePipeline(template_dir, registry, 'frontend_image', 'frontend_artifact', ['AWS_FRONTEND_REPOSITORY', 'frontend_react'] )
 
-    rendered_template_frontend = render_template("./src/templates/ci-pipeline/azure-pipelines.yaml", {
+    rendered_template_frontend = render_template(template_dir, "azure-pipelines.yaml", {
         'set_artifacts_build': phases_frontend[0],
         'get_artifacts_deploy': phases_frontend[1],
         'deploy_artifact': phases_frontend[2]
     })
     
     typer.echo(rendered_template_frontend)
 
     return rendered_template_frontend
 
 
-def mountAzurePipelineBackend(registry):
-    phases_api = mountAzurePipeline(registry, 'backend_fastapi', 'Fastapi_Artifact', ['AWS_API_REPOSITORY', 'backend_fastapi'] )
-    phases_data_migration = mountAzurePipeline(registry, 'frontend_image', 'frontend_artifact', ['AWS_FLYWAY_REPOSITORY', 'migrations_flyway'] )
+def mountAzurePipelineBackend(registry, template_dir):
+    phases_api = mountAzurePipeline(template_dir, registry, 'backend_fastapi', 'Fastapi_Artifact', ['AWS_API_REPOSITORY', 'backend_fastapi'] )
+    phases_data_migration = mountAzurePipeline(template_dir, registry, 'frontend_image', 'frontend_artifact', ['AWS_FLYWAY_REPOSITORY', 'migrations_flyway'] )
 
-    rendered_template_backend = render_template("./src/templates/ci-pipeline/azure-pipelines.yaml", {
+    rendered_template_backend = render_template(template_dir, "azure-pipelines.yaml", {
         'set_artifacts_build': phases_api[0] + phases_data_migration[0],
         'get_artifacts_deploy': phases_api[1] + phases_data_migration[1],
         'deploy_artifact': phases_api[2] + phases_data_migration[2]
     })
     
     typer.echo(rendered_template_backend)
 
     return rendered_template_backend
 
 
 
 
-def mountAzurePipeline(registry, artifact_tar, artifact_name, registry_variables ):
+def mountAzurePipeline(template_dir, registry, artifact_tar, artifact_name, registry_variables ):
+    
 
-    pipeline_build_template = render_template("./src/templates/ci-pipeline/set-artifact.yaml", {
+    pipeline_build_template = render_template(template_dir, "set-artifact.yaml", {
         'artifact_tar_name' : artifact_tar,
         'artifact_pipeline_name': artifact_name
     })
-    pipeline_get_artifact_file = render_template("./src/templates/ci-pipeline/get-artifact.yaml", {
+    pipeline_get_artifact_file = render_template(template_dir, "get-artifact.yaml", {
         'artifact_tar_name' : artifact_tar,
         'artifact_pipeline_name': artifact_name
     })
     
     if registry == "ECR (Elastic Container Registry)":
-        deploy_artifact_file = render_template("./src/templates/ci-pipeline/deploy-artifacts-ecr.yaml", {
+        deploy_artifact_file = render_template(template_dir, "deploy-artifacts-ecr.yaml", {
                 'repository_variable' : registry_variables[0],
                 'image_name' : registry_variables[1]
             })
     elif registry == "ACR (Azure Container Registry)":
         #To implement
         test = 1
     elif registry == "Docker Hub":
-        deploy_artifact_file = render_template("./src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml", {
+        deploy_artifact_file = render_template(template_dir, "deploy-artifacts-docker-hub.yaml", {
             'image_name' : registry_variables[0],
             'registry_username' : registry_variables[1],
             'registry_name' : registry_variables[2]
         })
 
     return [pipeline_build_template, pipeline_get_artifact_file, deploy_artifact_file]
 
 
 
-def load_template(template_file: str, variables: Dict[str, str]) -> str:
-    with open(template_file, "r") as file:
-        template = file.read()
-        filled_template = template.format(**variables)
-        return filled_template
+#def load_template(template_file: str, variables: Dict[str, str]) -> str:
+#    with open(template_file, "r") as file:
+#        template = file.read()
+#        filled_template = template.format(**variables)
+#        return filled_template
 
 # Helper function to save a filled template to a file
 def save_template(template: str, output_file: str):
     with open(output_file, "w") as file:
         file.write(template)
 
 
-def render_template(template_file, context):
-    file_loader = FileSystemLoader('.')
+def render_template(template_dir,template_file, context):
+    script_directory = os.path.dirname(os.path.abspath(__file__))
+    template_dir_source = os.path.join(script_directory, *template_dir)
+
+    file_loader = FileSystemLoader(template_dir_source)
     env = Environment(loader=file_loader)
+    #current_directory_source = os.path.dirname(os.path.abspath(__file__))
     template = env.get_template(template_file)
     rendered_template = template.render(context)
     return rendered_template
 
 #template_mappings = {
 #    "azure-pipelines.yaml": {"tests": "tests"},
 #    "steps_template.yaml": {}  # Add variables specific to the steps template
@@ -394,14 +408,35 @@
 
 def read_yaml(file_path):
     with open(file_path, "r") as file:
         yaml_data = yaml.safe_load(file)
     return yaml_data
 
 
+@app.command()
+def testee():
+    arr = ["templates","ci-pipeline"]
+    script_directory = os.path.dirname(os.path.abspath(__file__))
+    #template_dir = os.path.join(script_directory, "templates","ci-pipeline")
+    template_dir_source = os.path.join(script_directory, *arr)
+    typer.echo(script_directory)
+    typer.echo(template_dir_source)
+
+    file_loader = FileSystemLoader(template_dir_source)
+    env = Environment(loader=file_loader)
+    #current_directory_source = os.path.dirname(os.path.abspath(__file__))
+    template = env.get_template("set-artifact.yaml")
+    rendered_template = template.render({
+        'artifact_tar_name' : "artifact_tar",
+        'artifact_pipeline_name': "artifact_name"
+    })
+    typer.echo(rendered_template)
+
+
+
 
 
 
 @app.command()
 def template():
     source_file = "setup_template.yaml"
     destination_file = "downloaded_template.yaml"
```

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/argocd/argocd.yaml` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/argocd/argocd.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/blueprints.tf` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/blueprints.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/developer-role.tf` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/developer-role.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/kubernetes-addons.tf` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/kubernetes-addons.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/main.tf` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/main.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/values/vcluster-config-init.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/IaC/aws/vpc-module.tf` & `devopipe-0.1.5/devopipe/src/templates/IaC/aws/vpc-module.tf`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml` & `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/azure-pipelines.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml` & `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-docker-hub.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml` & `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/deploy-artifacts-ecr.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/ci-pipeline/get-artifact.yaml` & `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/get-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/ci-pipeline/set-artifact.yaml` & `devopipe-0.1.5/devopipe/src/templates/ci-pipeline/set-artifact.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/deployment.yaml` & `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml` & `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_backend.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/deployment_database.yaml` & `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/deployment_database.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml` & `devopipe-0.1.5/devopipe/src/templates/kubernetes/apps/pgadmin-deploy.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml` & `devopipe-0.1.5/devopipe/src/templates/kubernetes/aws/ingress_aws.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/tests/database-sonarqube.yaml` & `devopipe-0.1.5/devopipe/src/templates/tests/database-sonarqube.yaml`

 * *Files identical despite different names*

### Comparing `devopipe-0.1.4/devopipe/src/templates/tests/deployment-sonarqube.yaml` & `devopipe-0.1.5/devopipe/src/templates/tests/deployment-sonarqube.yaml`

 * *Files identical despite different names*

