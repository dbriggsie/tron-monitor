<h1 align="center">
  <img src="https://github.com/dbriggsie/tron-monitor/blob/master/tron-monitor.png">
  <br/>
  Tron Monitor
</h1>
Tron Monitor is a monitoring script built in Powershell for checking primary node uptime. This will be most useful for Tron Super Representatives & Tron Super Representative Candidates although anyone running a Tron Node can use it.


Examples of use:
  * If you have a secondary node ready for failover when primary node goes into offline state.
  
<br/>
<h3>Sponsors</h3>
No sponsors yet.. Will you be the first?

# How to use
Firstly, you will need to install powershell on the machine which will run your secondary **java-tron** node.
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
   
