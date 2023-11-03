<h1>Failed RDP Authentication by Geolocation</h1>

<h2>Description</h2>

• Setup Azure Sentinel (SIEM) and connected to a live virtual machine acting as a honey pot. Observed live attacks from all around the world. Used a custom PowerShell script to pinpoint attackers' geolocation information and plotted on the Azure Sentinel map.</br>

<h2>Utilities</h2>

• ipgeolocation.io

<h2>Steps</h2>

<h4>1. Create a virtual machine in Azure.</h4></br>

![image](https://github.com/thegreatkw/Sentinel_Lab/assets/128569887/435ba7c4-aae6-4eda-9e33-11a2807d2812)



<h4>2. Create log repository (Log Analytics Workspace)</h4></br>

![image](https://github.com/thegreatkw/Sentinel_Lab/assets/128569887/79215641-2592-49ca-83ad-bc05c9ff25c8)


<h4>3. Setup Microsoft Sentinel (cloud native SIEM)</h4></br>

![image](https://github.com/thegreatkw/Sentinel_Lab/assets/128569887/2d5d8def-cf70-4c96-9eab-1e0ff9def250)


<h4>4. Viewed attacks being logged from Japan</h4></br>

![image](https://github.com/thegreatkw/Sentinel_Lab/assets/128569887/f4a27636-6925-498e-bf41-aa7055e5201c)


<h4>5. Used powershell to extreact IP address from windows log and send to 3rd party api (ipgeolocation) for longitude and latitude information. Create a custom log with geographic data.</h4></br>

![image](https://github.com/thegreatkw/Sentinel_Lab/assets/128569887/542875d4-e419-440a-890b-30343644f70a)


