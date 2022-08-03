# Hadoop Installation Guide and HDFS Hands On - H1 (Homework)

Every step is to be executed on the home directory. Use `cd` to move to home directory.

The commands in the guide use ```USER``` as the notation for your username. If you have executed A0 correctly, then this should be your SRN in lowercase. This is important since the auto-evaluation depends on it. Verify your username by running `whoami` on the terminal.

Change any `/home/USER/` to `/home/<your SRN>/`

## This manual includes steps that you will be doing from your home since it involves downloading large files. This would not be possible in college due to the WiFi restrictions and speeds.

**The part which will be done in class will be shared later**

Execute the following commands to move to the home directory and updating the package list and the system. This guide assumes that you are working with Ubuntu or a Debian based distribution.
```bash
cd
sudo apt update -y
sudo apt upgrade -y
```
## Step 1 - Installing Java

Since Hadoop 3.3.3 may not support newer versions of Java, we install Java 8 using the following command.
```bash
sudo apt install openjdk-8-jdk -y
```

Check if Java is successfully installed and the version with the following commands.
```bash
java -version
javac -version
```

## Step 2 - Downloading Hadoop

Use the link given below to download and extract hadoop using the following commands.
```bash
cd
wget https://dlcdn.apache.org/hadoop/common/hadoop-3.3.3/hadoop-3.3.3.tar.gz
tar xzf /home/USER/hadoop-3.3.3.tar.gz
```