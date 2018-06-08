<h1 align="center">
  Tron Monitor
</h1>
Tron Monitor is a monitoring script built in Powershell for checking primary node uptime. This will be most useful for Tron Super Representative Candidates & Tron Super Representatives.

Examples of use:
  * if you have a secondary node ready for failover when primary node goes into offline state.

# How to use
Firstly, you will need to installing powershell on your node.
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
   
