<details>
<summary>Low Java Virtual Machine heap size</summary>
 
This occurs because the parameter for Java Virtual Machine (JVM) heap size is set to a min of 256m and a max of 512m as the default memory. When AMIMOSRV runs out of memory, the error message is displayed. 
Could we remove the duplicated sentence “runs out of memory the error message is displayed”? It appears twice in the above paragraph.
***Added new update here.***

**Solution**: To increase the JVM heap size that is located in the BMCSAMP dataset in MUXMONEV member.

In the following default parameter:

IJO="$IJO -Xms256m -Xmx512m"
Replace -Xms256m with Xms512m
Replace -Xmx512m with -Xmx1048m
</details >  

<details>
<summary>BMC AMI Ops User Interface not populating Host Server</summary>   


BMC AMI Ops User Interface not populating Host Server. This might happen if you are using a version earlier than Installation System 4.11.00.

**Solution**: Check whether the amisir64 library is present in your runtime file system. If not, manually copy the amisir64 library to the runtime environment.
 
</details>

<details>
<summary>Troubleshooting AT-TLS connections</summary>

To make sure that BMC AMI Ops User Interface receives expected data, configure the following for BMC AMI Ops User Interface and the BMC AMI Ops products:

Authorization—The Security definitions for BMC AMI Ops user interface branch lists topics about customizing authorization for RACF, ACF2, and Top Secret.
Alarm manager—Turn on Alarm manager and distribute alarms to be captured for the BMC AMI Ops User Interface dashboards and alarms. For more information about Alarm Management, see Using Alarm Management. For information about setting up configuring alarms for distribution, see Working with Alarm Management parameter files.

HFSPATH configuration—Configure the BMC AMI Ops CAS and PAS to point to the correct HFSPATH entries. For more information, see Identifying a file system to a CAS.
 
</details>


   
<summary>Prerequisites</summary>

1. Have committed your changes.   
2. Are connected to the correct remote repository.   
3. Have permission to push to the repository.


More testing of this wierd process........ :D
***Added new update here.***
Testing Done for latest review
