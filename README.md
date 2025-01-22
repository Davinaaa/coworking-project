1. Create an EKS Cluster
2. Update the Kubeconfig
3. Create YAML Configurations
4. Create PersistentVolumeClaim
5. Create PersistentVolume
6. Postgres Deployment
7. Apply YAML configurations
8. Test Database Connection
9. Run Seed Files
10. Deploy the Analytics Application
    - Dockerize the Application
    - Set up Continuous Integration with CodeBuild
    - Deploy the Application
    - Verify the Deployment

    docker build --platform linux/amd64 -t 721419945856.dkr.ecr.us-east-1.amazonaws.com/coworking-ecr-repo:0.0.10 -f analytics/Dockerfile .
docker push 721419945856.dkr.ecr.us-east-1.amazonaws.com/coworking-ecr-repo:0.0.10

abc1ddb2eaf764d5ea80dc6753258d66-493868280.us-east-1.elb.amazonaws.com
curl abc1ddb2eaf764d5ea80dc6753258d66-493868280.us-east-1.elb.amazonaws.com/api/reports/daily_usage

aws iam attach-role-policy \
--role-name eksctl-my-cluster-nodegroup-my-nod-NodeInstanceRole-qHzU1Q9OpS3S \
--policy-arn arn:aws:iam::aws:policy/CloudWatchAgentServerPolicy 

aws eks create-addon --addon-name amazon-cloudwatch-observability --cluster-name my-cluster
