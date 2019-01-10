---
title: 'Response status codes'

layout: nil
---

## Chapter 4 | Parameters

* Parameters provide required inputs to Cmdlets if needed. Few CmdLets do not require any inputs few have mandatory parameters
* Paremeters are provided using a `-` hyphon i.e. `Any-Cmdlet -Parameter1 -Parameter2`
* Parameter values are supplied through a `<space>` char.
* Example of such parameter is `Get-Process -Name svchost` here `-Name` is a Parameter and 'svchost' is its value.

* If you use a `Get-Help` and see the syntax section, you will see a list of parameters which you can supply to given CmdLet

![image](https://user-images.githubusercontent.com/13016162/50883084-fa1edb00-140c-11e9-873e-1bd549a2f2f2.png)

* If you directly supply parameter without using `-ParameterName` the first positional parameter will be considered as default

![image](https://user-images.githubusercontent.com/13016162/50894379-1597df00-1429-11e9-84ad-863597f0efad.png)

* Single-Value Vs Multi-Value Parameter | Notice `<string>` vs `<string[]>`

![image](https://user-images.githubusercontent.com/13016162/50893305-90abc600-1426-11e9-80c5-85763ec896bf.png)

* Help shows Parameter data type. 
* `<string>` is a single string i.e. Single Value can be supplied.
* `<string[]>` is an array of strings i.e. Multiple string values can be supplied
* Example `Test-Connection -ComputerName 127.0.0.1 10.0.0.1` here -ComputerName parameter is `<string[]>` type hence two IPs are supplied as input

![image](https://user-images.githubusercontent.com/13016162/50893776-aff72300-1427-11e9-9bdc-43c1fe13e339.png)

### Common Parameters

![image](https://user-images.githubusercontent.com/13016162/50883162-48cc7500-140d-11e9-91cd-35b15bb1d2a6.png)

* What and How many are these CommonParameters ?

```
 The common parameters are:
    -Verbose
    -Debug
    -WarningAction
    -WarningVariable
    -ErrorAction
    -ErrorVariable
    -OutVariable
    -OutBuffer
    
 The risk mitigation parameters are:
    -WhatIf
    -Confirm
```


