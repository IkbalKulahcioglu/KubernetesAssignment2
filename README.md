# kubernetes-assignment-2-IkbalKulahcioglu
kubernetes-assignment-2-IkbalKulahcioglu created by GitHub Classroom

Dockerfile oluşturduktan sonra aşağıdaki docker kodu ile docker image oluşturdum.

     docker build -t my-node-app:1.0 .


Deployment için .yaml dosyasını oluşturdum ve .yaml dosyasını kullanarak kubernetes ile deploymentı oluşturdum.

    kubectl apply -f my-app-deployment.yaml


Aşağıdakı komut ile ReplicaSetin çalıştığını kontrol ettim.

    kubectl get rs

Uygulamanin yük dengelemesi için LoadBalancer tipi bir Servis yaml dosyası oluşturdum. Komut ile Kubernetes de uyguladım.

    kubectl apply -f my-app-service.yaml

Yüksek erişilebilirliğini test etmek için Deployment'ı 5 pod'a ölçekledim.

    kubectl scale deployment my-app --replicas=5





Terminal çıktıları: 
![image](https://github.com/LOG-IN-DEVOPS-BOOTCAMP/kubernetes-assignment-2-IkbalKulahcioglu/assets/65568713/2f6fb99e-a9ec-4c71-9b56-930e23cc6ee2)
