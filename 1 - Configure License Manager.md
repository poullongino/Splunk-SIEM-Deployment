## Configuring License Manager and connecting all components to the License Manager

### In License Manager,

#### 1. Go to Settings --> Licensing --> "Change license group" --> "Enterprise License" --> Click on "Save".

![image](https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/346faf85-0b42-4d1d-946c-e2ed373af9b1)

 

#### 2. In Add new license page, Click on "Choose File" and Select your license and Click on "Install".

<img width="1191" alt="image" src="https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/6c6789d1-cbc0-4a1f-9b59-8cca20c0c05a">



#### 3. You need to restart the Splunk to make the changes reflected.

<img width="1191" alt="image" src="https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/163073c9-4e92-463e-8212-6111ee3ebe4c">



#### 4. Once restarted, you can verify the same in Settings --> Licensing.

<img width="1056" alt="image" src="https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/7305a163-a476-4a9c-93f8-b725123b7e77">



### In other components (Cluster Manager, Indexer 1, Indexer 2, Indexer 3, Search Head 1, Search Head 2, Search Head 3, Deployment Server, Intermediate Forwarder 1, Intermediate Forwarder 2),


#### 1. Go to Settings --> Licensing --> "Change to Peer".

<img width="1191" alt="image" src="https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/69e9e812-8294-42a1-82c9-2a6f1b8a5b99">



#### 2. Select “Designate a different Splunk instance as the manager license server” >> Add License_Manager's URl & management Port >> Save 

![image](https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/8253e0e8-829a-4142-b8b0-ac575dce529e)



#### 3. You need to restart the Splunk to make the changes reflected.

![image](https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/e20a80fc-eca1-4a5f-9b49-e0ad7131d107)



#### 4. Once restarted, you can verify the same in Settings --> Licensing.

![image](https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/db04f6ba-990b-41ff-8851-0a24bce4c0ab)


### To Check If all components are connected to License Manager,

#### 1. In License Manager, Go to Settings --> Licensing --> All indexer details (in the bottom page).

![image](https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/0848f192-ad3f-4e4f-a85b-1a0883bb32da)



#### 2. All the components should be listed here!

<img width="616" alt="image" src="https://github.com/SoftManiaTech/Splunk-SIEM-Deployment-Internal/assets/52287805/1f679a79-7c84-4d34-ae73-caa45a8f194f">


### License Manager is configured successfully.


