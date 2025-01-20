Hi, I have some issues I couldn't solve myself. I have tried for a long time but I can't make it. If you could check my code and screenshots and help me with them I will be super grateful, thank you.

I have two issues.

1. Couldn't deploy the application properly
After I applied the deployment.yaml file, I ran 'kubectl get deployments', I foud this:

workspace root$ kubectl get deployments
NAME         READY   UP-TO-DATE   AVAILABLE   AGE
coworking    0/1     1            0           25m
postgresql   1/1     1            1           8h

workspace root$ kubectl get pods
NAME                          READY   STATUS             RESTARTS      AGE
coworking-5479f4cdc8-7z985    0/1     CrashLoopBackOff   6 (70s ago)   26m
coworking-7c4f78c655-kpwjh    0/1     Error              2 (26s ago)   28s
postgresql-688c5c767c-rt7w8   1/1     Running            0             77m

You can see these errors in my screenshots as well. I tired a lot but still can't make it, please could you help me with some solutions? Thank you very much.


2. I couldn't find any clusters in the CloudWatch page.
Please check the 'screenshots/15 can't find my cluster in CloudWatch.png' screenshot. I'm not sure if it's because my deployment has not started well. Any thoughts will be very helpful, thank you so much.