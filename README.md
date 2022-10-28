# devops-bootcamp-project-6
Demo project for Module 9 - AWS services

1. create admin user with less privileges than root user and login to AWS with admin user
<img width="503" alt="Capture d’écran 2022-10-26 à 16 53 43" src="https://user-images.githubusercontent.com/62488871/198060205-87d33c7d-4aed-4c68-9dfd-8b92d9c3854e.png">

2. Create EC2 instance
<img width="1196" alt="Capture d’écran 2022-10-26 à 17 11 15" src="https://user-images.githubusercontent.com/62488871/198064806-5832fbcf-778b-4ae9-955b-722a531e65b8.png">

3. SSH into instance
<img width="285" alt="Capture d’écran 2022-10-26 à 17 30 06" src="https://user-images.githubusercontent.com/62488871/198069411-cbe35775-0870-4129-8b3f-bab9398c7110.png">

4. Update package manager tool, install Docker, start Docker daemon, add user to group to run Docker cmd without sudo

5. Pull image from Docker hub containing web app
<img width="668" alt="Capture d’écran 2022-10-27 à 18 57 27" src="https://user-images.githubusercontent.com/62488871/198353971-6ce26677-a1ca-46b0-8f3f-744019152e46.png">

6. Config firewall of instance to make app accessible from browser and run container
<img width="1135" alt="Capture d’écran 2022-10-27 à 19 00 46" src="https://user-images.githubusercontent.com/62488871/198353988-7136fbeb-5cb5-4e4f-ba46-20a234910150.png">
<img width="516" alt="Capture d’écran 2022-10-27 à 19 01 29" src="https://user-images.githubusercontent.com/62488871/198353996-811dc3bf-b5f3-46d7-8a84-98873cc5d109.png">

7. Install SSH agent plugin on Jenkins & add SSH key for EC2 instance login in Jenkins credentials

8. Add SSH login and run Docker img logic to Jenkinsfile (need to enable SSH access for EC2 instance on port 22)
<img width="713" alt="Capture d’écran 2022-10-28 à 19 33 32" src="https://user-images.githubusercontent.com/62488871/198699568-1824254c-14bc-424c-a895-1066941dd70a.png">

9. Run Jenkins build on pipeline and check that app is running on server
<img width="916" alt="Capture d’écran 2022-10-28 à 20 09 42" src="https://user-images.githubusercontent.com/62488871/198704077-d02ddffc-849b-462b-994f-93675c24761d.png">

