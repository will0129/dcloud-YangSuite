# dcloud-YangSuite

## Purpose

The Dcloud Yangsuite lab is an environment with a prebuilt and integrated Yangsuite system so that people can evaluate yangsuite. It can be used for teams that cannot install yangsuite in their corporate environment due to controls in place, or who do not have an appropriate backend (routes/switches) to evaluate yangsuite against. 

It includes a prebuilt yangsuite and the below devices
c8kv
c9kv
CSR
IOS-XR Virtual router
NX-OS Virtual device

All devices except the CSR are preconfigured into Yangsuite, the CSR is not currently loaded because (1) there is already an IOS_XE device and (2) this allows users to evaluate the workflow of onboarding a device into yangsuite.

There is also a Jupyter notebook with python examples of using restconf, so the intent is you could use the example that uses the IETF-interfaces model, and manipulate it with other models from yangsuite (as you wish), and interrogate them in the python environment.

![image](https://user-images.githubusercontent.com/32154829/226478130-6bae5158-886b-4f1c-b13e-4ce85e12ee5e.png)

All Usernames: admin
All Passwords: C1sco12345

Yangsuite (when in via VPN)
https://198.18.133.100:8443/

![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/2aa415d0-855b-44f0-b5a1-84987df1fcbe)



## Using the lab

Schedule the Dcloud instance with your Cisco technical team. they can share the lab with you.

Note the c9kv Virtual machine is not, always performant or stable. There is no production use case for it (since c8kv is by design software intended, c9k is hardware optimized), so it was never made production ready. It was working and the yang models were cloned, but it may not always work and future iterations will likely have a better build. 

I prefer, anyconnect method. Where you vpn into the environment and run RDP locally from your machine. You can also do web RDP. Both examples are expanded on below...

To connect via anyconnect use the info and anyconnect info to the left.

![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/4791927f-ebf0-419d-8204-3e17822f07a5)

to connect to yangsuite via webRDP, you would select the yangsuite device and webRDP from the left 


![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/a2bc8ac9-8ed0-4bcf-9ffa-dc331e8999d1)



Launch the browser, restore tabs or dont. use the link provided to access yangsuite.

![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/a1dfdb8d-26bf-43b4-a214-19b2fc812cf3)


![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/9872bc98-70dd-436e-9eda-c1ef1ea1417b)

Devices are already loaded, 

![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/d69641c0-48bd-4ab4-8f66-a9b188a93bd0)

To access the example python scripts you click launch jupyter notebook desktop icon and then you can open the scripts.

![image](https://github.com/will0129/dcloud-YangSuite/assets/32154829/30d4e713-7283-4a33-b226-d1de524af422)






