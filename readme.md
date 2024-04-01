# GCP-VPC-documentation

### Select project
1. Open the Google Cloud Platform (GCP) console.
2. Select the desired project.

<img src="https://github.com/mindmotivate/GCP_private/assets/130941970/64bfc3e7-aece-4ffc-8eb2-9ab62d301188" width="50%" height="50%">

### Go to search bar
3. Type in VPC networks and click on "VPC networks in the drop down list.

insert pic

4. Before you do anything, you will see a 'default' network under the VPC networks section.  DO NOT DELETE the default network

### Create VPC Network
5. Click on 'CREATE VPC NETWORK' near the top of the page.  You will go to the creation page.

insert

6. Name your VPC and give it a description (optional)
7. Under 'VPC network ULA internal IPv6 range' section, leave that disabled
8. Under 'Subnets' section, leave it checked on custom.
9. Under 'New subnet', give it a name, description (optional), and specify a region.
10. Under 'IP stack type', leave it checked on IPv4 (single stack)
11. Enter your designated IP range value in the 'IPv4 range' field

insert pic

12. Do not touch the 'Create Secondary IPV4 Range' button.
13. Under 'Private Google Access', click 'On'.
14. Under 'Flow logs', click 'On'.  We don't have to configure logs
15. Under 'Hybrid subnet'. leave that checked at 'Off'.
16. We are not adding another subnet at this time.  Do not touch 'Add Subnet'.
17. Under <b>'Firewall rules'</b> section, there is a list of rules as depicted below.  Let's check the 'allow-icmp' to allow your network to return pings. Check the 'allow-ssh' to allow an SSH connection to your network.

insert pic

18. Under 'Dynamic routing mode', leave it checked on 'Regional' since we are using a single region for our VPC and VM.
19. Click on 'Create'

insert pic

