# webgoat init.d script
This is a working init.d script to be used with any init based linux system. Especially created for Amazon AMI Instances in EC2.

It launches the standalone WebGoat container that is supposed to be in the home folder of the user ec2-user. 

Replace $PATH_TO_JAR with the filename/version you are using.

The script obviously is going to /etc/init.d. Verify the file mode bits are set correct.

For the Amazon AMI add the script to the init system using this command:

```
ec2$ sudo chkconfig --add webgoat
```

Based this stackoverflow question: http://bit.ly/29AlvpQ

Have fun.
