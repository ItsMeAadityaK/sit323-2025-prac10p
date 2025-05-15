1. First, I logged into the Google Cloud Console and created a Standard Kubernetes Cluster named sit323-cluster.
2. While setting up the cluster, I selected the australia-southeast2 region and used a regional configuration.
3. To ensure that full monitoring metrics like CPU and memory usage would be available, I used the appropriate command to increase the cluster’s node count to 3 after deployment.
4. Once the cluster was ready, I verified that my student account was active and selected the correct project sit323-25t1-kulkarni-c60fbf8.
5. I reused my calculator microservice from earlier tasks and updated the code by disabling MongoDB integration and the /history route.
6. I built the Docker image locally and pushed it to my Docker Hub account under the updated tag for use in this task.
7. After that, I created Kubernetes YAML files for deployment and service. These were applied to the cluster using kubectl, and I confirmed that the pods reached the Running state.
8. I accessed the microservice through the External IP assigned by the LoadBalancer and verified that all calculator endpoints worked successfully.
9. To set up monitoring, I navigated to Google Cloud Console → Monitoring → Metrics Explorer.
10. I selected Kubernetes Container as the resource type and visualized key metrics such as:

CPU utilization
Memory usage
Ingress packet count
Log entry count

11. I also used Logs Explorer to query application logs filtered by cluster name, container name, and namespace.
12. All required monitoring data and logs were successfully displayed, and screenshots were captured showing metric graphs, pod activity, and external IP access.
13. The task was completed successfully with proper observability and monitoring set up using GCP tools.