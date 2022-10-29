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

10. Install docker-compose on ec2 instance
<img width="669" alt="Capture d’écran 2022-10-29 à 15 14 31" src="https://user-images.githubusercontent.com/62488871/198833597-1b8d8931-698a-409f-b2f9-dfa1e98ccba0.png">

11. Create docker-compose file
<img width="633" alt="Capture d’écran 2022-10-29 à 15 23 31" src="https://user-images.githubusercontent.com/62488871/198833930-6027af93-892f-4df4-84f5-0356732985b0.png">

12. Adjust Jenkinsfile for docker-compose -> copy docker-compose file from repo to ec2 instance, ssh into instance and run docker-compose file on instance
<img width="753" alt="Capture d’écran 2022-10-29 à 15 33 43" src="https://user-images.githubusercontent.com/62488871/198834741-0ce08310-2668-4abb-bcdc-6ddfce51a281.png">

13. Run Jenkins build and check relevant containers are running on ec2 instance and that docker-compose file is there
<img width="588" alt="Capture d’écran 2022-10-29 à 15 33 31" src="https://user-images.githubusercontent.com/62488871/198834708-51a6864e-d22b-4dda-9120-108f9f848ce7.png">
<img width="673" alt="Capture d’écran 2022-10-29 à 15 34 05" src="https://user-images.githubusercontent.com/62488871/198834726-ff6ffe89-3d91-4037-8683-27c749fa76a5.png">

14. Parameterise docker image tag in Dockerfile
<img width="640" alt="Capture d’écran 2022-10-29 à 16 08 57" src="https://user-images.githubusercontent.com/62488871/198836264-843985a9-c7fb-48f2-a745-0c3f1afb9b96.png">
<img width="387" alt="Capture d’écran 2022-10-29 à 16 08 47" src="https://user-images.githubusercontent.com/62488871/198836279-bca16dc9-d989-4168-b876-eb4fa235879d.png">
<img width="495" alt="Capture d’écran 2022-10-29 à 16 12 46" src="https://user-images.githubusercontent.com/62488871/198836245-25ad395b-fbcd-40d2-a805-82dcd15cb5de.png">
<img width="640" alt="Capture d’écran 2022-10-29 à 16 08 57" src="https://user-images.githubusercontent.com/62488871/198836264-843985a9-c7fb-48f2-a745-0c3f1afb9b96.png">
<img width="495" alt="Capture d’écran 2022-10-29 à 16 12 46" src="https://user-images.githubusercontent.com/62488871/198836245-25ad395b-fbcd-40d2-a805-82dcd15cb5de.png">

