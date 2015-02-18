# selenium
selenium

Issues faced in launching Selenium test case on below setup:  

Windows Server 2008  
Bamboo Elastic Agent  
IEdriverserver.exe - 32 bit   

Update below settings on the Bamboo account used by the build server: 


1. HKEY_CURRENT_USER\Software\Microsoft\Internet Explorer\Main 
[STRING]TabProcGrowth  1   [NOT DWORD]

2. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Internet Explorer\Main\FeatureControl\FEATURE_BFCACHE 
[DWORD]iexplore.exe 0

3. IE Advanced options -> Enable Enhanced Protected Mode OFF

4. Disable Protected mode on all four Zones in IE options

5. Enable .Net Framework on custom level
