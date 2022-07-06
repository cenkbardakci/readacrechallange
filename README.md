# Test Project

Python - Flask Web App, which reads the current RAM and CPU usage and a React frontend which shows the statistics in the browser
# Test Project

Python - Flask Web App, which reads the current RAM and CPU usage and a React frontend which shows the statistics in the browser

# Dockerized and Build
docker build -f Dockerfile.api -t red-acre-app-api .
docker build -f Dockerfile.client -t red-acre-frontend .
docker-compose up


# If ports conflict
docker-compose down
docker rm -fv $(docker ps -aq)
sudo lsof -i -P -n | grep 5000

# Terraform run eks cluster


# initialize terraform configuration
terraform init

# validate terraform configuration
terraform validate

# create terraform plan
terraform plan -out state.tfplan

# apply terraform plan
terraform apply state.tfplan

# cleanup
terraform destroy -auto-approve
