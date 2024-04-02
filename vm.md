# Placing a VM (Virtual Machine) in the VPC That We Created

### Creating a VM (Virtual Machine)
You must be working from the same Google Cloud project as the one you created your VPC in.
1. Type in 'vm instance' in the search bar near the top of the page. Click on 'Add VM instance' in the list of items in the drop down box.

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-01%20compute%20engine%20vm.PNG">

2. The first thing we will do is give your VM a name.  Then specify a <b>Region</b> and <b>Zone</b> for your VM.

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-02%20name%20and%20region.PNG">

3. Under the <b>'Machine Configuration'</b> section, we will leave the selection on E2 for this instance.

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-03%20machine%20configuration%201.PNG">

4. We will leave ALL options alone as we scroll down to the <b>Firewall</b> section since we are doing a simple VM instance.  Click a check on the 'Allow HTTP traffic' option.  <i>(I checked the 'Allow HTTPS traffic' option for the certain results of this specific VM URL)</i>

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-04%20Firewall.PNG">

5. Next, click on the arrow next to the <b>Advanced options</b> to expand the options. Underneath, click on the arrow next to the  <b>Networking</b> section to expand the networking options.  Scroll down to the <b>Network interfaces</b> section.  Click on the 'Network' field under 'Edit network interface'.  You should be able to choose the VPC you created. Then scroll down to the 'Done' button and click.

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-05%20network%20interface.PNG">

6. Next, click on the arrow next to the <b>Management</b> to expand the options.  Scroll down to the <b>Automation</b> field. Copy and paste the startup script you have in the field. We don't have to touch anything else.

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-06%20startup%20script.PNG">

7. Click on the blue <b>'Create'</b> button at the bottom of the screen to create your VM.
8. When the instance is done being created, copy the 'External IP' for your VM instance address on the 'WM instances' page.  Use 'http://   ' and the external IP address that was copied to paste and open in the browswer. The code in your startup script should dictate the contents of your published website that is run from the VM in your VPC network.

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/-07%20external%20ip.PNG">

<img src="https://github.com/dn30001/GCP-VPC-documentation/blob/main/The%20Resulting%20Screenshot.PNG">
  
