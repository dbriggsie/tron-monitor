<h1 align="center">
  <img src="https://github.com/dbriggsie/tron-monitor/blob/master/tron-monitor.png">
  <br/>
  Tron Monitor
</h1>
Tron Monitor is a monitoring script built in Powershell to check and monitor that your SR Node is producing blocks. The script will send an email alert to you if your node hasn't produced blocks for over 2 minutes. This will be most useful for Tron Super Representatives & Tron Super Representative Candidates, although anyone running a Tron Node can use it to prepare themselves for being voted into top 27 as an SR.



  
### Sponsors
No sponsors yet.. Will you be the first? <br/>
**`Sponsors get access to (pre-releases) with new features - potential to stay ahead of the competition.`**
<br/>

# How to use
You are not obligated to run the tron-monitor script on the same system that runs your witness node.
Firstly, you will need to install powershell on the machine which you choose to monitor your **java-tron** witness node from.

   ## Installing Powershell on Ubuntu 16.04
      # Import the public repository GPG keys
        curl https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -

      # Register the Microsoft Ubuntu repository
        curl https://packages.microsoft.com/config/ubuntu/16.04/prod.list | sudo tee /etc/apt/sources.list.d/microsoft.list

      # Update apt-get
        sudo apt-get update

      # Install PowerShell
        sudo apt-get install -y powershell

      # Start PowerShell
        powershell
  
## Forking the Tron Monitor code using git
      # git clone https://github.com/dbriggsie/tron-monitor.git
      
## Configuring Tron Monitor
     
      # Change into Tron Monitor Directory
        cd tron-monitor/
        sudo vi tron-monitor.ps1
        
   **`EDIT THE FOLLOWING CONFIG LINES IN THE SCRIPT TO YOUR NEEDS. MAKE SURE TO CHANGE TO YOUR SR NODES WITNESS ADDRESS`**

      #Please Change the Producerkey to your own Witness Address.
      $ProducerKey = "TAbzgkG8p3yF5aywKVgq9AaAu6hvF2JrVC"

      # Configure this Minute value, so that script can run on this interval, 5 value denotes that script will wait for 5 minute 
      # to re-check, Change according to the requirement can be any decimal value 1,2,3,4,5 etc...
      $CheckAfterEveryMin = 1

      #Configure the from email id
      $EmailFrom = "user@domain.net"

      #Configure email id to whom you want to send email
      $EmailTo = "user@domain.net"

      #Configure the subject line
      $EmailSubject = "[Alert] Witness Node has Stopped Producing Blocks"

      #Configure SMTP server either name or IP address 
      $SMTPServer = "smtphost.domain.net"

      #Default SMTP port is 25 but incase SMTP is running on any other port, configure this $smtpport value
      $SMTPPort = 25

      #Configure the user name who is authorized to send an email
      $SMTPAuthUsername = "username"

      #Configure password of the user
      $SMTPAuthPassword = "password"

      #Configure the Settings to use SSL
      $UseSSL = $true

      #Configure the body text of the email
      $emailbody = "[Alert] Witness Node has Stopped Producing Blocks"


## Running Tron Monitor
      # Change into Tron Monitor Directory
        cd tron-monitor/
        
      # Change Permissions to enable running
        sudo chmod +x tron-monitor.ps1
        
      # Start Powershell
        powershell
        
      # Execute Tron Monitor
        ./tron-monitor.ps1
        
## Donate
   If you found this script helpful and want to donate, please use the following **ERC20 TRX address.**
   `0x5d262a24f65cf80098c8032454722eca0449d78e`
