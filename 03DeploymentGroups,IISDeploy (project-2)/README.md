## git Hub ##
https://github.com/vipin-k/eShopLegacyWebForms

## create new repo on azure devops and push the code.

## create CI pipeline and create the artifact
# create pipeline using the classic editor
# select ASP.NET template
# remove test assemblies
# then run the pipeline

# create new VM in azure 
# Go to azure devops and click on deployment group and create new group called dev.
# Login the VM and copy the powershell script and execute on the VM.
# Make the VM as IIS server. 
# To do that Go to server manager and click on add "roles and features". under server role select "web server IIS" option. And install the IIS protocol.
# Go start button and type IIS manager, this should be available. 
# click on explore and get the files. and check the applications.
# we can access this application outside of the server using the public IP.

## release pipeline ##
# create new release pipeline, select template "IIS website deployment". 
# remote iis webapp manage task.
# under iis deployment select your deployment group.
# check all the information and create release. After the release pipeline completed, you can actually see the application has been deployed successfully on the target folder.