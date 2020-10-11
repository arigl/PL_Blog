Navigating the painstaking install process of Haskell:

If you are struggling to install Haskell, you are not alone.
Especially on Windows machines, installing Haskell can be very challenging, especially if you skip directions and dont install specific prerequisites. 
On Mac machines, this process is fairly easy and can be done without many hiccups, so refer to haskells website and you should be fine. 

1. Install Choclatey

- Travel to this site: https://chocolatey.org/install 
- Open up Powershell as administrator.
- Paste this code in:
  - Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
- Wait for a few seconds, and check to make sure it is properly installed with choco or choco -?

2. Install Haskell

- In your admin powershell prompt, run this code:
  - choco install haskell-dev
- Then after this has finished, run this code:
  - refreshenv
  
3. Test to make sure it is working

- You should now be able to type in ghci without any problems. 
- The lines should preface with Prelude>
- Go ahead and try out some basic math functions to get a grasp of what Haskell is capable of, and what it is not. 
