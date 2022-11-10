# Geoserver

This solution uses Jenkins to automatically deploy a containerized (docker) build of Geoserver to Microsoft Azure. Since Jenkins runs on a local system, in a real-world deployment scenario, a dedicated server would need to be in place. Various cost and scalibility considerations would also need to be made in order to determine whether this solution, or a cloud based CI/CD deployment pipeline solution, is the best approach for a given company/organization.

The server can be accessed at [http://geoserver-jelson.eastus.azurecontainer.io:8080/geoserver](http://geoserver-jelson.eastus.azurecontainer.io:8080/geoserver) with the following credentials:
- Username: admin
- Password: IS27-SPA

### Requirements

- [Docker](https://docs.docker.com/desktop/install/linux-install/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- [Jenkins](https://docs.docker.com/compose/install/)

### How to Use

Place the geoserver-deploy folder into the jobs folder of your Jenkins installation (e.g. /var/lib/jenkins/jobs).

Ensure Jenkins is running:

    sudo systemctl start jenkins

Then run the job in Jenkins to automate a deployment.

## Resources Used

- [https://github.com/geoserver/docker](https://github.com/geoserver/docker)
- [https://docs.docker.com/cloud/aci-integration/](https://docs.docker.com/cloud/aci-integration/)

