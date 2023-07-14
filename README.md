# EnsHelper
IRIS Integration Extensions and Utilities 

# Install
```
zpm install alwo-enshelper
```

# Class - HostRequestResponseInfo
Extend a custom BusinessService, BusinessHost or BusinessOperation.<br/>
When Instance Settings of a custom class are viewed in Production on Management Portal, this helper adds two new fields to the "Information" section.<br/>
These fields show the Request Message Types and Response Message Types, consumed and returned by the production instance.

![Image Show Request Response Types](/img/HostRequestResponseInfo.png)

## How to implement
To use simply add this class name to the Extends list in class definition of any custom Service, Process or Operation type<br/>
Business Service
```objectScript
Class myService extends (Ens.BusinessService, alwo.EnsHelper.HostRequestResponseInfo)
{
  ...
}
```
Business Process
```objectScript
Class myBusinessProcess extends (Ens.BusinessProcess, alwo.EnsHelper.HostRequestResponseInfo)
{
  ...
}
```

```objectScript
Class myOperation extends (Ens.BusinessOperation, alwo.EnsHelper.HostRequestResponseInfo)
{
  ...
}
```

