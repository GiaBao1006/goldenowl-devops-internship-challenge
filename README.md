[intern.drawio](https://github.com/user-attachments/files/23354295/intern.drawio)# Golden Owl DevOps Internship - Technical Test
Submitted by: Nguyen Gia Bao (GiaBao1006)

## Your Mission 🌟
Your mission, should you choose to accept it, is to craft a CI job that:
1. Forks this repository to your personal GitHub account.
2. Dockerizes a Node.js application.
3. Establishes an automated CI/CD build process using GitHub Actions workflow and a container registry service such as DockerHub or Amazon Elastic Container Registry (ECR) or similar services.
4. Initiates CI tests automatically when changes are pushed to the feature branch on GitHub.
5. Utilizes GitHub Actions for Continuous Deployment (CD) to deploy the application to major cloud providers like AWS EC2, AWS ECS or Google Cloud (please submit the deployment link).

## Tech Stack
1. Cloud: AWS (Amazon Web Services)
        Compute: EC2 (Elastic Compute Cloud)
        Networking: VPC, Subnets, Route Tables, Internet Gateway, ALB
        Scaling & HA: Auto Scaling Group (ASG)
        Container Registry: ECR (Elastic Container Registry)

2. Infrastructure as Code: Terraform

3. Containerization: Docker

4. CI/CD: GitHub Actions

5. Application: Node.js

## Architecture Diagram

[Uploading inte<mxfile host="Electron" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) draw.io/27.0.9 Chrome/134.0.6998.205 Electron/35.4.0 Safari/537.36" version="27.0.9">
  <diagram name="Page-1" id="7bMH3r9v7BJEo7vAqxY3">
    <mxGraphModel dx="996" dy="771" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="RQXClBrlCKCKh2q2imq--18" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="RQXClBrlCKCKh2q2imq--1" target="RQXClBrlCKCKh2q2imq--2">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--1" value="User" style="sketch=0;outlineConnect=0;fontColor=#232F3E;gradientColor=none;strokeColor=#232F3E;fillColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.user;" vertex="1" parent="1">
          <mxGeometry x="63.18" y="150" width="60" height="60" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--2" value="Internet&lt;div&gt;&lt;br&gt;&lt;/div&gt;" style="image;aspect=fixed;perimeter=ellipsePerimeter;html=1;align=center;shadow=0;dashed=0;spacingTop=3;image=img/lib/active_directory/internet_cloud.svg;" vertex="1" parent="1">
          <mxGeometry x="41.58999999999999" y="272.5" width="103.18" height="65" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--4" value="AWS Cloud" style="points=[[0,0],[0.25,0],[0.5,0],[0.75,0],[1,0],[1,0.25],[1,0.5],[1,0.75],[1,1],[0.75,1],[0.5,1],[0.25,1],[0,1],[0,0.75],[0,0.5],[0,0.25]];outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;container=1;pointerEvents=0;collapsible=0;recursiveResize=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_aws_cloud_alt;strokeColor=#232F3E;fillColor=none;verticalAlign=top;align=left;spacingLeft=30;fontColor=#232F3E;dashed=0;" vertex="1" parent="1">
          <mxGeometry x="200" y="70" width="630" height="470" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--6" value="Public subnet" style="points=[[0,0],[0.25,0],[0.5,0],[0.75,0],[1,0],[1,0.25],[1,0.5],[1,0.75],[1,1],[0.75,1],[0.5,1],[0.25,1],[0,1],[0,0.75],[0,0.5],[0,0.25]];outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;container=1;pointerEvents=0;collapsible=0;recursiveResize=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_security_group;grStroke=0;strokeColor=#7AA116;fillColor=#F2F6E8;verticalAlign=top;align=left;spacingLeft=30;fontColor=#248814;dashed=0;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="300" y="50" width="130" height="130" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--8" value="EC2" style="sketch=0;points=[[0,0,0],[0.25,0,0],[0.5,0,0],[0.75,0,0],[1,0,0],[0,1,0],[0.25,1,0],[0.5,1,0],[0.75,1,0],[1,1,0],[0,0.25,0],[0,0.5,0],[0,0.75,0],[1,0.25,0],[1,0.5,0],[1,0.75,0]];outlineConnect=0;fontColor=#232F3E;fillColor=#ED7100;strokeColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.ec2;" vertex="1" parent="RQXClBrlCKCKh2q2imq--6">
          <mxGeometry x="35" y="35" width="60" height="60" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--7" value="Public subnet" style="points=[[0,0],[0.25,0],[0.5,0],[0.75,0],[1,0],[1,0.25],[1,0.5],[1,0.75],[1,1],[0.75,1],[0.5,1],[0.25,1],[0,1],[0,0.75],[0,0.5],[0,0.25]];outlineConnect=0;gradientColor=none;html=1;whiteSpace=wrap;fontSize=12;fontStyle=0;container=1;pointerEvents=0;collapsible=0;recursiveResize=0;shape=mxgraph.aws4.group;grIcon=mxgraph.aws4.group_security_group;grStroke=0;strokeColor=#7AA116;fillColor=#F2F6E8;verticalAlign=top;align=left;spacingLeft=30;fontColor=#248814;dashed=0;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="300" y="300" width="130" height="130" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--9" value="EC2" style="sketch=0;points=[[0,0,0],[0.25,0,0],[0.5,0,0],[0.75,0,0],[1,0,0],[0,1,0],[0.25,1,0],[0.5,1,0],[0.75,1,0],[1,1,0],[0,0.25,0],[0,0.5,0],[0,0.75,0],[1,0.25,0],[1,0.5,0],[1,0.75,0]];outlineConnect=0;fontColor=#232F3E;fillColor=#ED7100;strokeColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.ec2;" vertex="1" parent="RQXClBrlCKCKh2q2imq--7">
          <mxGeometry x="35" y="35" width="60" height="60" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--20" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="RQXClBrlCKCKh2q2imq--4" source="RQXClBrlCKCKh2q2imq--10" target="RQXClBrlCKCKh2q2imq--6">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--23" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.5;entryY=1;entryDx=0;entryDy=0;" edge="1" parent="RQXClBrlCKCKh2q2imq--4" source="RQXClBrlCKCKh2q2imq--10" target="RQXClBrlCKCKh2q2imq--7">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--10" value="ALB" style="points=[];aspect=fixed;html=1;align=center;shadow=0;dashed=0;fillColor=#FF6A00;strokeColor=none;shape=mxgraph.alibaba_cloud.alb_application_load_balancer_02;spacing=8;spacingTop=110;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="50" y="197.5" width="75" height="75" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--22" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.5;entryY=1;entryDx=0;entryDy=0;" edge="1" parent="RQXClBrlCKCKh2q2imq--4" source="RQXClBrlCKCKh2q2imq--11" target="RQXClBrlCKCKh2q2imq--6">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--24" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="RQXClBrlCKCKh2q2imq--4" source="RQXClBrlCKCKh2q2imq--11" target="RQXClBrlCKCKh2q2imq--7">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--11" value="ASG" style="outlineConnect=0;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;shape=mxgraph.aws3.auto_scaling;fillColor=#F58534;gradientColor=none;spacingTop=5;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="460" y="187.5" width="80" height="85" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--13" value="ECR" style="sketch=0;points=[[0,0,0],[0.25,0,0],[0.5,0,0],[0.75,0,0],[1,0,0],[0,1,0],[0.25,1,0],[0.5,1,0],[0.75,1,0],[1,1,0],[0,0.25,0],[0,0.5,0],[0,0.75,0],[1,0.25,0],[1,0.5,0],[1,0.75,0]];outlineConnect=0;fontColor=#232F3E;fillColor=#ED7100;strokeColor=#ffffff;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;shape=mxgraph.aws4.resourceIcon;resIcon=mxgraph.aws4.ecr;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="540" y="335" width="60" height="60" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--25" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="RQXClBrlCKCKh2q2imq--4" source="RQXClBrlCKCKh2q2imq--8" target="RQXClBrlCKCKh2q2imq--13">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--26" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0;entryY=0.5;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="RQXClBrlCKCKh2q2imq--4" source="RQXClBrlCKCKh2q2imq--9" target="RQXClBrlCKCKh2q2imq--13">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--37" value="Distribution" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="125" y="197.5" width="80" height="30" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--38" value="Manages EC2" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="RQXClBrlCKCKh2q2imq--4">
          <mxGeometry x="360" y="197.5" width="100" height="30" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--34" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="1" source="RQXClBrlCKCKh2q2imq--15" target="RQXClBrlCKCKh2q2imq--11">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--39" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="1" source="RQXClBrlCKCKh2q2imq--15" target="RQXClBrlCKCKh2q2imq--13">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--15" value="GitHub Actions&amp;nbsp;" style="dashed=0;outlineConnect=0;html=1;align=center;labelPosition=center;verticalLabelPosition=bottom;verticalAlign=top;shape=mxgraph.weblogos.github" vertex="1" parent="1">
          <mxGeometry x="440" y="600" width="70" height="65" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--33" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="1" source="RQXClBrlCKCKh2q2imq--16" target="RQXClBrlCKCKh2q2imq--15">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--16" value="Dev&lt;div&gt;&lt;br&gt;&lt;/div&gt;" style="sketch=0;outlineConnect=0;fontColor=#232F3E;gradientColor=none;fillColor=#232F3D;strokeColor=none;dashed=0;verticalLabelPosition=bottom;verticalAlign=top;align=center;html=1;fontSize=12;fontStyle=0;aspect=fixed;pointerEvents=1;shape=mxgraph.aws4.user;" vertex="1" parent="1">
          <mxGeometry x="200" y="602.5" width="60" height="60" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--19" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0.027;entryY=0.507;entryDx=0;entryDy=0;entryPerimeter=0;" edge="1" parent="1" source="RQXClBrlCKCKh2q2imq--2" target="RQXClBrlCKCKh2q2imq--10">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--35" value="Push code" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="310" y="600" width="80" height="30" as="geometry" />
        </mxCell>
        <mxCell id="RQXClBrlCKCKh2q2imq--36" value="Build and Push&lt;div&gt;CI/CD&lt;/div&gt;" style="text;html=1;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;strokeColor=none;fillColor=none;" vertex="1" parent="1">
          <mxGeometry x="550" y="590" width="100" height="40" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
rn.drawio…]()


## How To Deploy
Prerequisites:
    Terraform CLI installed.
    AWS CLI installed and configured.
    Docker installed and running.

### 1. Terraform (Infrastructure):

Navigate to the terraform directory and apply the configuration to create the AWS infrastructure.

1. Navigate to the terraform directory
cd terraform
2. Initialize Terraform
terraform init
3. (Optional) Plan the changes
terraform plan
4. Apply the configuration to create the infrastructure
terraform apply


### 2. Docker (Manual Build & Push for First Deployment):

This is required one time to give the EC2 instances an image to pull.
Note: You must replace [ACCOUNT_ID], [REGION], and [ECR_REPOSITORY_URL] with your actual values from the terraform output.

1. Navigate to the root directory (where the Dockerfile is)
cd ..
2. Log in to Amazon ECR
aws ecr get-login-password --region [REGION] | docker login --username AWS --password-stdin [ACCOUNT_ID].dkr.ecr.[REGION].amazonaws.com
3. Build the Docker image (for the EC2 platform, linux/amd64)
docker buildx build --platform linux/amd64 -t [ECR_REPOSITORY_URL]:latest .
4. Push the image to ECR
docker push [ECR_REPOSITORY_URL]:latest


### 3. GitHub CI/CD Pipeline:

CI (Continuous Integration): Automatically runs npm test on every Pull Request to ensure code quality.

CD (Continuous Deployment): Automatically builds, pushes, and deploys the application with zero-downtime (via Rolling Update) on every merge to the master branch.

## Important
Create a new user in the IAM console with AmazonEC2ContainerRegistryFullAccess and AutoScalingFullAccess policies. Then, create an Access Key and Secret Key for this user and add them to the GitHub repository's Secrets (AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY, AWS_REGION, ASG_NAME). This is required for the CD pipeline to work.

## Clean all
cd terraform
terraform destroy #Destroy the Terraform-managed infrastructure
