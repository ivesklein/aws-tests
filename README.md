# EC2

1. Log to the console
2. go to ec2 service
3. go to the desired zone
4. go to instances
5. click launch instance
6. select Ubuntu Server xx.xx LTS
7. in step 3 you can choose the subnet(each in different availability zone)
8. in step x you can set the `Name` tag to difference your instance
9. in step 6 you assign the aws firewall config, for example you can add http & https ports to can provide a webserver
10. click launch, here aws ask for a key pair, it is for ssh access.
11. download the key
12. click view instances
13. select the instance you created
14. in description copy the "IPv4 Public IP"
15. change the permisions of the downloaded key to 400(means just user can read)
16. in the terminal write `ssh -i theKeyFile.pem ubuntu@CopiedPublicIP`
17. Now you are inside the instance
