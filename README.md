##### FuzzPy
FuzzPy is a Simple and Basic Library writing in python3, and aims to simple the action of finding Urls with Parameter for Enumartion Step in Pen-Testing for specific Scope. The Original Code and Tool has Been Developed Under the Name of Photon "https://github.com/s0md3v/Photon" . i Should also Refrence that the module SCARPY "https://scrapy.org/"  is also Another Powerfull Library that also includes a pythonic Spider/Crawler but the use of this Simple Library is Only and Only for Development the "Scoped-Base Penetration Testing Tools". 

#### Usage 
Usage of the Library is Very Simple and it can be used just in few lines 
```
from fuzzpylib import Crawler as cr 
TARGET ='blablabla.com'
a = Crawler(TARGET , crawl_level = 2)
data = a.launch()
print(data)
```
also the data in which is returned is a Dictionary in which there are two Keys 
  - 'fuzzable' 
  - 'internal'
  
```
from fuzzpylib import Crawler as cr 
TARGET ='blablabla.com'
a = Crawler(YOUR_TAGET , crawl_level = 2 , thread_num = 10 , user_agent = "YOUR USER AGENT" , moderator = None ,
			 exclude = None , timeout = 10)
data = a.launch()
print(data)
```
  - crawl_level : Levels To Crawl
  - thread_num : Number of Threads 
  - user_agent : User Agent 
  - moderator : Out_Put_Control / (default is None and None is python 'print'  function)
  - exclude : Exclude Any Adress from scope 
  - timeout : Requests Time out 
##### Notes : 

  - This Project is Sub-Project of XFramework : https://github.com/r3dxpl0it/Xframwork
  - This Crawler Does not Bypass DNS firewall 
  - Always be Aware of IpTables and dont use it Blindly 
