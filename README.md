# aws-cloud9-playground

learn [AWS Cloud9](https://aws.amazon.com/cloud9/)

## Enabling SSH Connectivity

* add SSH inbound rule to Security Group
    ![](https://www.evernote.com/l/AAEY_BSM7g5PVa72gIFEevDXgdKE1E-zAdoB/image.png)
* add `~/.ssh/id_rsa.pub` to `/home/ec2-user/.ssh/authorized_keys`.  do this via Cloud9 IDE shell
    ![](https://www.evernote.com/l/AAGhf-SuVVRDtpS8fMS9lRQmHCwQSs6A1v8B/image.png)
* ssh -i ~/.ssh/id_rsa  ec2-user@ec2-34-226-142-54.compute-1.amazonaws.com

> NOTE: may need to connect via Cloud9 IDE to "wake up"/start instance due to "auto stop" of EC2 instance after
X minutes.

## VS Code Remote Development on Cloud9

* perform "Enabling SSH Connectivity" steps
* see [vscode | Remote development over SSH](https://code.visualstudio.com/docs/remote/ssh-tutorial)


## Resources

* [VS Code Remote Development](https://code.visualstudio.com/docs/remote/remote-overview)
* [vscode | Remote development over SSH](https://code.visualstudio.com/docs/remote/ssh-tutorial)