                            **EKS-2048-Game**

          In this Repo we will be deploying 2048 Game

Pre-requisites:

1. AWS account
2. CLI installed
3. eksctl
4. kubectl
5. Common sense


Step:1 Create cluster using CLI of instance type fargate.

![Screenshot 2024-02-20 171507](https://github.com/hijackhim/EKS-2048-Game/assets/105789918/539fed02-f75a-4b3f-9851-b94367a2bcb2)

Step:2 Create fargate profile using file "Game-app_ingress.md".

![Screenshot 2024-02-20 171614](https://github.com/hijackhim/EKS-2048-Game/assets/105789918/331224d3-87b4-4540-b029-afe04eff6b4c)

Step:3 Now create and apply services, deployment and ingress from the file "sampleapp.md".

![Screenshot 2024-02-20 171257](https://github.com/hijackhim/EKS-2048-Game/assets/105789918/4e8b95bc-ee68-4031-8f3b-cef85a26884e)

Step:4 Now install IAM OIDC provider from file "OIDC-connector.md".

Step:5 Now create IAM policy using file "ALB controller-addon.md" for ALB controller as pre-requisite.

Step:6 Now create a role from file "ALB controller-addon.md".

Step:7 Now install ALB controller from helm chart using the file "ALB controller-addon.md".

Step:8 We will get the DNS address from load-balancer to access our game from anywhere.

![Screenshot 2024-02-20 171332](https://github.com/hijackhim/EKS-2048-Game/assets/105789918/b1b12e10-f556-49ae-8c56-b018a0c438f9)

![image](https://github.com/hijackhim/EKS-2048-Game/assets/105789918/63de487e-7202-4486-9a5d-fd16cc223143)

![image](https://github.com/hijackhim/EKS-2048-Game/assets/105789918/b2d212c9-8ee3-41e9-9cfc-e1cb40636fd1)
