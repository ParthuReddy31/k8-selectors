## Selectors

taint node 
cmd  
kubectl taint nodes ip-192-168-39-127.ec2.internal hardware=gpu:NoSchedule
kubectl taint nodes ip-192-168-49-64.ec2.internal hardware=gpu:NoExecute


untaint:
kubectl taint nodes ip-192-168-39-127.ec2.internal hardware=gpu:NoSchedule-
kubectl taint nodes ip-192-168-49-64.ec2.internal hardware=gpu:NoExecute-

kubectl taint nodes ip-192-168-39-127.ec2.internal hardware=gpu:NoExecute


before affinity you have to label the nodes:
kubectl label nodes ip-192-168-39-127.ec2.internal hardware=gpu
kubectl label nodes ip-192-168-49-64.ec2.internal hardware=gpu