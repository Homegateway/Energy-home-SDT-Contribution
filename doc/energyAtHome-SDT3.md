

# Domain "domain1"

## Devices


### root1


#### Modules


##### AffectedParametersList  
<p>A list of parameters affected by a compatibility control action</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceParameters|Array *ApplianceParameters*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameter*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ApplianceParameterTable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *permissions*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NameListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *id*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveApplianceParameterSettingsLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NameListLink*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### Appliance  
<p>An appliance is any kind of smart home device</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|loadShedDeviceCategory|array *loadShedDeviceCategory*|Yes|Yes|Yes|Yes| |
|sFDI|integer *sFDI*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|ActiveApplianceControlListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceControlListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceLogEventListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceMonitorListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceParameterCompatibilityActionListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceParameterListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceWorkingModeListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceStatisticListLink|uri |Yes|Yes|Yes|Yes| |
|ConfigurationLink|uri |Yes|Yes|Yes|Yes| |
|DERListLink|uri |Yes|Yes|Yes|Yes| |
|DeviceInformationLink|uri |Yes|Yes|Yes|Yes| |
|DeviceStatusLink|uri |Yes|Yes|Yes|Yes| |
|FileStatusLink|uri |Yes|Yes|Yes|Yes| |
|IPInterfaceListLink|uri |Yes|Yes|Yes|Yes| |
|LoadShedAvailabilityLink|uri |Yes|Yes|Yes|Yes| |
|LogEventListLink|uri |Yes|Yes|Yes|Yes| |
|PowerStatusLink|uri |Yes|Yes|Yes|Yes| |
|ExtendedPowerProfileListLink|uri |Yes|Yes|Yes|Yes| |


##### ApplianceControlList  
<p>A List of Appliance Controls</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteApplianceControl|href:&nbsp;string *href* |No| |
|None|CreateApplianceControl|ApplianceControl:&nbsp;Struct *ApplianceControl*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Array *ApplianceParameterStates*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameterState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *now*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceControls|Array *ApplianceControls*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceControl*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *ApplianceParameterStates*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameterState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *now*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceMonitorList  
<p>A list of Appliance Monitors</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceMonitors|Array *ApplianceMonitors*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceMonitor*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ApplianceParameterState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *now*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxValue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *minValue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceParameterCompatibilityActionList  
<p>A list of Appliance Parameter Compatibility Actions</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceParameterCompatibilityActions|Array *ApplianceParameterCompatibilityActions*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameterCompatibilityAction*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *action*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Expressions*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Expression*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *logicalConnective*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *mathOperator*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *max*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *AffectedParametersListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceParameterList  
<p>A List of Appliance Parameters</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceParameters|Array *ApplianceParameters*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameter*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ApplianceParameterTable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *permissions*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NameListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *id*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveApplianceParameterSettingsLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NameListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceParameterSetList  
<p>A List of Appliance Parameter Sets</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceParameterSets|Array *ApplianceParameterSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameterSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *ApplianceParameterSettingss*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceParameterSettings*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *AvoidedValues*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *AvoidedValue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *default*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *max*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *min*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Expressions*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Expression*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *logicalConnective*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *mathOperator*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceWorkingModeList  
<p>A list of Appliance Working Modes</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceWorkingModes|Array *ApplianceWorkingModes*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceWorkingMode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *name*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *id*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceParameterSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NameListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### LocalNameList  
<p>A List of names associated with an object, used for internazionalization</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|LocalNames|Array *LocalNames*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *LocalName*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *name*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *language*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceStatisticList  
<p>A List element to hold ApplianceStatistic objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ApplianceStatistics|Array *ApplianceStatistics*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ApplianceStatistic*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *applianceStatisticID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *applianceStatisticPayload*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *timeStamp*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|applianceStatisticListMaxSize|integer *applianceStatisticListMaxSize*|No|Yes|Yes|Yes| |
|applianceStatisticMaxSize|integer *applianceStatisticMaxSize*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ExtendedPowerProfileList  
<p>A List of Extended Power Profiles for a device</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|energyRemote|boolean *energyRemote*|No|Yes|Yes|Yes| |
|ExtendedPowerProfiles|Array *ExtendedPowerProfiles*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ExtendedPowerProfile*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *PowerProfiles*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *PowerProfile*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *alternativeModesNumber*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *minPowerProfileDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *mixEnable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Modes*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Mode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *EnergyPhases*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *EnergyPhase*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *SignedRealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *expectedDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *macroPhaseID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxActivationDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxAnticipation*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxOverloadPause*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *EnergyPhaseScheduleStateLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *repetitionNumber*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *all*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *results*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ExtendedPowerProfilePriceLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerProfileScheduleContraintsLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerProfileScheduleStateLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerProfileStateLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *results*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *all*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|multipleScheduling|boolean *multipleScheduling*|No|Yes|Yes|Yes| |
|totalProfileNum|integer *totalProfileNum*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ExtendedPowerProfilePrice  
<p>Price of an Extended Power Profile</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|currency|integer *currency*|No|Yes|Yes|Yes| |
|price|integer *price*|No|Yes|Yes|Yes| |
|pricePowerOfTenMultiplier|integer *pricePowerOfTenMultiplier*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### OverallSchedulePrice  
<p>Cost associated to all the Extended Power Profiles scheduled for the next 24 hours.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|currency|integer *currency*|No|Yes|Yes|Yes| |
|price|integer *price*|No|Yes|Yes|Yes| |
|pricePowerOfTenMultiplier|integer *pricePowerOfTenMultiplier*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PowerProfileSchedule  
<p>Schedule for an Extended Power Profile</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|PowerProfileScheduleLists|Array *PowerProfileScheduleLists*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *PowerProfileScheduleList*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *minPowerProfileDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *PowerProfileScheduleModes*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *PowerProfileScheduleMode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *EnergyPhaseSchedules*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *EnergyPhaseSchedule*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *activationDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *EnergyPhaseLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ModeLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *all*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *results*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PowerProfileScheduleContraints  
<p>Scheduling constraints of a Power Profile</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|scheduleMode|array *scheduleMode*|No|Yes|Yes|Yes| |
|startAfter|integer *startAfter*|No|Yes|Yes|Yes| |
|stopBefore|integer *stopBefore*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PowerProfileScheduleState  
<p>Actual scheduling state of a Power Profile</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|CreatePowerProfileScheduleState|PowerProfileScheduleState:&nbsp;Struct *PowerProfileScheduleState*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *minPowerProfileDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Array *PowerProfileScheduleModeStates*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *PowerProfileScheduleModeState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *EnergyPhaseScheduleStates*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *EnergyPhaseScheduleState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *activationDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *EnergyPhaseLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ModeLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *all*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *results*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|minPowerProfileDelay|integer *minPowerProfileDelay*|No|Yes|Yes|Yes| |
|PowerProfileScheduleModeStates|Array *PowerProfileScheduleModeStates*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *PowerProfileScheduleModeState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *EnergyPhaseScheduleStates*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *EnergyPhaseScheduleState*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *activationDelay*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *EnergyPhaseLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ModeLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PowerProfileState  
<p>Actual state of a Power Profile</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|remoteControl|boolean *remoteControl*|No|Yes|Yes|Yes| |
|state|integer *state*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|ActiveEnergyPhaseLink|uri |Yes|Yes|Yes|Yes| |


##### DeviceCapability  
<p>Returned by the URI provided by DNS\-SD, to allow clients to find the URIs to the resources in which they are interested.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|href|string *href*|No|Yes|Yes|Yes| |
|EndDeviceListLink|uri |Yes|Yes|Yes|Yes| |
|MirrorUsagePointListLink|uri |Yes|Yes|Yes|Yes| |
|SelfDeviceLink|uri |Yes|Yes|Yes|Yes| |
|CustomerAccountListLink|uri |Yes|Yes|Yes|Yes| |
|DemandResponseProgramListLink|uri |Yes|Yes|Yes|Yes| |
|DERProgramListLink|uri |Yes|Yes|Yes|Yes| |
|FileListLink|uri |Yes|Yes|Yes|Yes| |
|MessagingProgramListLink|uri |Yes|Yes|Yes|Yes| |
|PrepaymentListLink|uri |Yes|Yes|Yes|Yes| |
|ResponseSetListLink|uri |Yes|Yes|Yes|Yes| |
|TariffProfileListLink|uri |Yes|Yes|Yes|Yes| |
|TimeLink|uri |Yes|Yes|Yes|Yes| |
|UsagePointListLink|uri |Yes|Yes|Yes|Yes| |


##### DeviceStatus  
<p>Status of device</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|changedTime|integer *changedTime*|No|Yes|Yes|Yes| |
|onCount|integer *onCount*|Yes|Yes|Yes|Yes| |
|opState|integer *opState*|Yes|Yes|Yes|Yes| |
|opTime|integer *opTime*|Yes|Yes|Yes|Yes| |
|Temperature|Struct *Temperature*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subject*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|TimeLink|uri |Yes|Yes|Yes|Yes| |


##### EndDeviceList  
<p>A List element to hold EndDevice objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteEndDevice|href:&nbsp;string *href* |Yes| |
|None|CreateEndDevice|EndDevice:&nbsp;Struct *EndDevice*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *OverallSchedulePricelink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *loadShedDeviceCategory*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *sFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ExtendedPowerProfilePriceLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *FlowReservationRequestListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *FlowReservationResponseListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *FunctionSetAssignmentsListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerProfileScheduleLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *RegistrationLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *SubscriptionListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceStatisticListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ConfigurationLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DeviceInformationLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DeviceStatusLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *FileStatusLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *IPInterfaceListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *LoadShedAvailabilityLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *LogEventListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerStatusLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|EndDevices|Array *EndDevices*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *EndDevice*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *OverallSchedulePricelink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *loadShedDeviceCategory*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *sFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ExtendedPowerProfilePriceLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *FlowReservationRequestListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *FlowReservationResponseListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *FunctionSetAssignmentsListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerProfileScheduleLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *RegistrationLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *SubscriptionListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ApplianceStatisticListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ConfigurationLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DeviceInformationLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DeviceStatusLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *FileStatusLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *IPInterfaceListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *LoadShedAvailabilityLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *LogEventListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PowerStatusLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### Registration  
<p>Registration represents an authorization to access the resources on a host.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|dateTimeRegistered|integer *dateTimeRegistered*|No|Yes|Yes|Yes| |
|pIN|integer *pIN*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### SelfDevice  
<p>The EndDevice providing the resources available within the DeviceCapabilities.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|loadShedDeviceCategory|array *loadShedDeviceCategory*|Yes|Yes|Yes|Yes| |
|sFDI|integer *sFDI*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|ExtendedPowerProfileListLink|uri |Yes|Yes|Yes|Yes| |
|ApplianceStatisticListLink|uri |Yes|Yes|Yes|Yes| |
|ConfigurationLink|uri |Yes|Yes|Yes|Yes| |
|DERListLink|uri |Yes|Yes|Yes|Yes| |
|DeviceInformationLink|uri |Yes|Yes|Yes|Yes| |
|DeviceStatusLink|uri |Yes|Yes|Yes|Yes| |
|FileStatusLink|uri |Yes|Yes|Yes|Yes| |
|IPInterfaceListLink|uri |Yes|Yes|Yes|Yes| |
|LoadShedAvailabilityLink|uri |Yes|Yes|Yes|Yes| |
|LogEventListLink|uri |Yes|Yes|Yes|Yes| |
|PowerStatusLink|uri |Yes|Yes|Yes|Yes| |


##### FunctionSetAssignmentsList  
<p>A List element to hold FunctionSetAssignments objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|FunctionSetAssignmentss|Array *FunctionSetAssignmentss*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *FunctionSetAssignments*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *CustomerAccountListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DemandResponseProgramListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERProgramListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *FileListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *MessagingProgramListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PrepaymentListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ResponseSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *TariffProfileListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *TimeLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *UsagePointListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### SubscriptionList  
<p>A List element to hold Subscription objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteSubscription|href:&nbsp;string *href* |No| |
|None|CreateSubscription|Subscription:&nbsp;Struct *Subscription*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Condition*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *attributeIdentifier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *lowerThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *upperThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *encoding*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *level*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *limit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *notificationURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *subscribedResource*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Subscriptions|Array *Subscriptions*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *Subscription*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Condition*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *attributeIdentifier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *lowerThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *upperThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *encoding*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *level*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *limit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *notificationURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *subscribedResource*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### NotificationList  
<p>A List element to hold Notification objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|CreateNotification|Notification:&nbsp;Struct *Notification*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *newResourceURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Resource*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *subscriptionURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *subscribedResource*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Notifications|Array *Notifications*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *Notification*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *newResourceURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Resource*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *subscriptionURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *subscribedResource*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ResponseList  
<p>A List element to hold Response objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteResponse|href:&nbsp;string *href* |Yes| |
|None|CreateResponse|Response:&nbsp;Struct *Response*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *createdDateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *endDeviceLFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *subject*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Responses|Array *Responses*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *Response*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *createdDateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *endDeviceLFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *subject*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ResponseSetList  
<p>A List element to hold ResponseSet objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ResponseSets|Array *ResponseSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ResponseSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ResponseListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### Time  
<p>Contains the representation of time, constantly updated.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|currentTime|integer *currentTime*|No|Yes|Yes|Yes| |
|dstEndTime|integer *dstEndTime*|No|Yes|Yes|Yes| |
|dstOffset|integer *dstOffset*|No|Yes|Yes|Yes| |
|dstStartTime|integer *dstStartTime*|No|Yes|Yes|Yes| |
|lastSetTime|integer *lastSetTime*|Yes|Yes|Yes|Yes| |
|localTime|integer *localTime*|Yes|Yes|Yes|Yes| |
|quality|integer *quality*|No|Yes|Yes|Yes| |
|tzOffset|integer *tzOffset*|No|Yes|Yes|Yes| |
|validUntilTime|integer *validUntilTime*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DeviceInformation  
<p>Contains identification and other information about the device that changes very infrequently, typically only when updates are applied, if ever.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|brandID|integer *brandID*|Yes|Yes|Yes|Yes| |
|brandName|string *brandName*|Yes|Yes|Yes|Yes| |
|CECEDSpecificationVersion|integer *CECEDSpecificationVersion*|Yes|Yes|Yes|Yes| |
|companyName|string *companyName*|Yes|Yes|Yes|Yes| |
|DRLCCapabilities|Struct *DRLCCapabilities*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *optionsImplemented*|Yes|Yes|Yes|Yes| |
|functionsImplemented|array *functionsImplemented*|Yes|Yes|Yes|Yes| |
|lFDI|array *lFDI*|No|Yes|Yes|Yes| |
|mfDate|integer *mfDate*|No|Yes|Yes|Yes| |
|mfHwVer|string *mfHwVer*|No|Yes|Yes|Yes| |
|mfID|integer *mfID*|No|Yes|Yes|Yes| |
|mfInfo|string *mfInfo*|Yes|Yes|Yes|Yes| |
|mfModel|string *mfModel*|No|Yes|Yes|Yes| |
|mfSerNum|string *mfSerNum*|No|Yes|Yes|Yes| |
|primaryPower|integer *primaryPower*|No|Yes|Yes|Yes| |
|productTypeID|integer *productTypeID*|Yes|Yes|Yes|Yes| |
|productTypeName|string *productTypeName*|Yes|Yes|Yes|Yes| |
|secondaryPower|integer *secondaryPower*|No|Yes|Yes|Yes| |
|swActTime|integer *swActTime*|No|Yes|Yes|Yes| |
|swVer|string *swVer*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|SupportedLocaleListLink|uri |Yes|Yes|Yes|Yes| |


##### SupportedLocaleList  
<p>A List element to hold SupportedLocale objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteSupportedLocale|href:&nbsp;string *href* |No| |
|None|CreateSupportedLocale|SupportedLocale:&nbsp;Struct *SupportedLocale*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *locale*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|SupportedLocales|Array *SupportedLocales*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *SupportedLocale*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *locale*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PowerStatus  
<p>Contains the status of the device's power sources</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|batteryStatus|integer *batteryStatus*|No|Yes|Yes|Yes| |
|changedTime|integer *changedTime*|No|Yes|Yes|Yes| |
|currentPowerSource|integer *currentPowerSource*|No|Yes|Yes|Yes| |
|estimatedChargeRemaining|integer *estimatedChargeRemaining*|Yes|Yes|Yes|Yes| |
|estimatedTimeRemaining|integer *estimatedTimeRemaining*|Yes|Yes|Yes|Yes| |
|PEVInfo|Struct *PEVInfo*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *minimumChargingDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *targetStateOfCharge*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *timeChargeIsNeeded*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *timeChargingStatusPEV*|Yes|Yes|Yes|Yes| |
|sessionTimeOnBattery|integer *sessionTimeOnBattery*|Yes|Yes|Yes|Yes| |
|totalTimeOnBattery|integer *totalTimeOnBattery*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### IPAddrList  
<p>List of IPAddr instances.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteIPAddr|href:&nbsp;string *href* |Yes| |
|None|CreateIPAddr|IPAddr:&nbsp;Struct *IPAddr*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *address*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *RPLInstanceListLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|IPAddrs|Array *IPAddrs*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *IPAddr*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *address*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *RPLInstanceListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### IPInterfaceList  
<p>List of IPInterface instances.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteIPInterface|href:&nbsp;string *href* |Yes| |
|None|CreateIPInterface|IPInterface:&nbsp;Struct *IPInterface*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *ifDescr*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifHighSpeed*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInBroadcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifIndex*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInDiscards*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInErrors*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInMulticastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInOctets*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInUcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInUnknownProtos*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifMtu*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *ifName*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOperStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutBroadcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutDiscards*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutErrors*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutMulticastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutOctets*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutUcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;- boolean *ifPromiscuousMode*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifSpeed*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifType*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastResetTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastUpdatedTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *IPAddrListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *LLInterfaceListLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|IPInterfaces|Array *IPInterfaces*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *IPInterface*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *ifDescr*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifHighSpeed*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInBroadcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifIndex*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInDiscards*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInErrors*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInMulticastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInOctets*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInUcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifInUnknownProtos*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifMtu*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *ifName*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOperStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutBroadcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutDiscards*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutErrors*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutMulticastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutOctets*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifOutUcastPkts*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *ifPromiscuousMode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifSpeed*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *ifType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastResetTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastUpdatedTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *IPAddrListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *LLInterfaceListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### LLInterfaceList  
<p>List of LLInterface instances.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteLLInterface|href:&nbsp;string *href* |Yes| |
|None|CreateLLInterface|LLInterface:&nbsp;Struct *LLInterface*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *CRCerrors*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *EUI64*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *IEEE_802_15_4*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *capabilityInfo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *shortAddress*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NeighborListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *linkLayerType*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLAckNotRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLCSMAFail*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesDropRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesDropTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLMediaAccessFail*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLOctetsRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLOctetsTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLRetryCount*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLSecurityErrorRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *loWPAN*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *octetsRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *octetsTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *packetsRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *packetsTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rxFragError*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|LLInterfaces|Array *LLInterfaces*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *LLInterface*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *CRCerrors*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *EUI64*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *IEEE_802_15_4*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *capabilityInfo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *shortAddress*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *NeighborListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *linkLayerType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLAckNotRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLCSMAFail*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesDropRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesDropTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLFramesTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLMediaAccessFail*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLOctetsRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLOctetsTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLRetryCount*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *LLSecurityErrorRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *loWPAN*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *octetsRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *octetsTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *packetsRx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *packetsTx*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rxFragError*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### NeighborList  
<p>List of 15.4 neighbors.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteNeighbor|href:&nbsp;string *href* |Yes| |
|None|CreateNeighbor|Neighbor:&nbsp;Struct *Neighbor*<br />&nbsp;&nbsp;&nbsp;&nbsp;- boolean *isChild*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *linkQuality*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *shortAddress*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Neighbors|Array *Neighbors*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *Neighbor*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *isChild*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *linkQuality*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *shortAddress*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### RPLInstanceList  
<p>List of RPLInstances associated with the IPinterface.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteRPLInstance|href:&nbsp;string *href* |Yes| |
|None|CreateRPLInstance|RPLInstance:&nbsp;Struct *RPLInstance*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *DODAGid*<br />&nbsp;&nbsp;&nbsp;&nbsp;- boolean *DODAGroot*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *flags*<br />&nbsp;&nbsp;&nbsp;&nbsp;- boolean *groundedFlag*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *MOP*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *PRF*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *rank*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *RPLInstanceID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *versionNumber*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *RPLSourceRoutesListLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|RPLInstances|Array *RPLInstances*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *RPLInstance*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *DODAGid*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *DODAGroot*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *flags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *groundedFlag*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *MOP*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *PRF*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rank*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *RPLInstanceID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *versionNumber*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *RPLSourceRoutesListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### RPLSourceRoutesList  
<p>List or RPL source routes if the hosting device is the DODAGroot</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteRPLSourceRoutes|href:&nbsp;string *href* |Yes| |
|None|CreateRPLSourceRoutes|RPLSourceRoutes:&nbsp;Struct *RPLSourceRoutes*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *DestAddress*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *SourceRoute*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|RPLSourceRoutess|Array *RPLSourceRoutess*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *RPLSourceRoutes*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *DestAddress*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *SourceRoute*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ApplianceLogEventList  
<p></p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteLogEvent|href:&nbsp;string *href* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|LogEvents|Array *LogEvents*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *LogEvent*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *createdDateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *extendedData*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *functionSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventCode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventPEN*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *profileID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### LogEventList  
<p>A List element to hold LogEvent objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteLogEvent|href:&nbsp;string *href* |No| |
|None|CreateLogEvent|LogEvent:&nbsp;Struct *LogEvent*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *createdDateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *extendedData*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *functionSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventCode*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventPEN*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *profileID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|LogEvents|Array *LogEvents*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *LogEvent*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *createdDateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *extendedData*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *functionSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventCode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *logEventPEN*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *profileID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### Configuration  
<p>This resource contains various settings to control the operation of the device</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|currentLocale|string *currentLocale*|No|Yes|Yes|Yes| |
|PowerConfiguration|Struct *PowerConfiguration*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *batteryInstallTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *lowChargeThreshold*|Yes|Yes|Yes|Yes| |
|TimeConfiguration|Struct *TimeConfiguration*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *dstEndRule*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dstOffset*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *dstStartRule*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *tzOffset*|Yes|Yes|Yes|Yes| |
|userDeviceName|string *userDeviceName*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|PriceResponseCfgListLink|uri |Yes|Yes|Yes|Yes| |


##### PriceResponseCfgList  
<p>A List element to hold PriceResponseCfg objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeletePriceResponseCfg|href:&nbsp;string *href* |No| |
|None|CreatePriceResponseCfg|PriceResponseCfg:&nbsp;Struct *PriceResponseCfg*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumeThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxReductionThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *RateComponentLink* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|PriceResponseCfgs|Array *PriceResponseCfgs*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *PriceResponseCfg*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumeThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxReductionThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *RateComponentLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### FileList  
<p>A List element to hold File objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Files|Array *Files*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *File*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *activateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *fileURI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *lFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *mfHwVer*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *mfID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *mfModel*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *mfSerNum*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *mfVer*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *size*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *type*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### FileStatus  
<p>This object provides status of device file load and activation operations.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|activateTime|integer *activateTime*|Yes|Yes|Yes|Yes| |
|loadPercent|integer *loadPercent*|No|Yes|Yes|Yes| |
|nextRequestAttempt|integer *nextRequestAttempt*|No|Yes|Yes|Yes| |
|request503Count|integer *request503Count*|No|Yes|Yes|Yes| |
|requestFailCount|integer *requestFailCount*|No|Yes|Yes|Yes| |
|status|integer *status*|No|Yes|Yes|Yes| |
|statusTime|integer *statusTime*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|FileLink|uri |Yes|Yes|Yes|Yes| |


##### DemandResponseProgramList  
<p>A List element to hold DemandResponseProgram objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|DemandResponsePrograms|Array *DemandResponsePrograms*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *DemandResponseProgram*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *availabilityUpdatePercentChangeThreshold*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *primacy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveEventListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *EventListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### EndDeviceControlList  
<p>A List element to hold EndDeviceControl objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|EndDeviceControls|Array *EndDeviceControls*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *EndDeviceControl*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ApplianceLoadReduction*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *type*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *deviceCategory*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *drProgramMandatory*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DutyCycle*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *normalValue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *loadShiftForward*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Offset*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *coolingOffset*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *heatingOffset*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *loadAdjustmentPercentageOffset*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *overrideDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *SetPoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *coolingSetpoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *heatingSetpoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *TargetReduction*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *type*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeStart*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### LoadShedAvailability  
<p>Indicates current consumption status and ability to shed load.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|availabilityDuration|integer *availabilityDuration*|Yes|Yes|Yes|Yes| |
|sheddablePercent|integer *sheddablePercent*|Yes|Yes|Yes|Yes| |
|sheddablePower|Struct *sheddablePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|DemandResponseProgramLink|uri |Yes|Yes|Yes|Yes| |


##### MeterReadingList  
<p>A List element to hold MeterReading objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteMeterReading|href:&nbsp;string *href* |Yes| |
|None|CreateMeterReading|MeterReading:&nbsp;Struct *MeterReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *RateComponentListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingTypeLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|MeterReadings|Array *MeterReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *MeterReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *RateComponentListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingTypeLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ReadingList  
<p>A List element to hold Reading objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteReading|href:&nbsp;string *href* |Yes| |
|None|CreateReading|Reading:&nbsp;Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Readings|Array *Readings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ReadingSetList  
<p>A List element to hold ReadingSet objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteReadingSet|href:&nbsp;string *href* |Yes| |
|None|CreateReadingSet|ReadingSet:&nbsp;Struct *ReadingSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingListLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ReadingSets|Array *ReadingSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ReadingSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ReadingType  
<p>Type of data conveyed by a specific Reading. See IEC 61968 Part 9 Annex C for full definitions of these values.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|accumulationBehaviour|integer *accumulationBehaviour*|Yes|Yes|Yes|Yes| |
|calorificValue|Struct *calorificValue*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|commodity|integer *commodity*|Yes|Yes|Yes|Yes| |
|conversionFactor|Struct *conversionFactor*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|dataQualifier|integer *dataQualifier*|Yes|Yes|Yes|Yes| |
|flowDirection|integer *flowDirection*|Yes|Yes|Yes|Yes| |
|intervalLength|integer *intervalLength*|Yes|Yes|Yes|Yes| |
|kind|integer *kind*|Yes|Yes|Yes|Yes| |
|maxNumberOfIntervals|integer *maxNumberOfIntervals*|Yes|Yes|Yes|Yes| |
|numberOfConsumptionBlocks|integer *numberOfConsumptionBlocks*|Yes|Yes|Yes|Yes| |
|numberOfTouTiers|integer *numberOfTouTiers*|Yes|Yes|Yes|Yes| |
|phase|integer *phase*|Yes|Yes|Yes|Yes| |
|powerOfTenMultiplier|integer *powerOfTenMultiplier*|Yes|Yes|Yes|Yes| |
|subIntervalLength|integer *subIntervalLength*|Yes|Yes|Yes|Yes| |
|supplyDisconnectLimit|integer *supplyDisconnectLimit*|Yes|Yes|Yes|Yes| |
|supplyLimit|integer *supplyLimit*|Yes|Yes|Yes|Yes| |
|supplyWarningLimit|integer *supplyWarningLimit*|Yes|Yes|Yes|Yes| |
|tieredConsumptionBlocks|boolean *tieredConsumptionBlocks*|Yes|Yes|Yes|Yes| |
|uom|integer *uom*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### UsagePointList  
<p>A List element to hold UsagePoint objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteUsagePoint|href:&nbsp;string *href* |Yes| |
|None|CreateUsagePoint|UsagePoint:&nbsp;Struct *UsagePoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *roleFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *serviceCategoryKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *MeterReadingListLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|UsagePoints|Array *UsagePoints*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *UsagePoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *roleFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *serviceCategoryKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *MeterReadingListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ConsumptionTariffIntervalList  
<p>A List element to hold ConsumptionTariffInterval objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ConsumptionTariffIntervals|Array *ConsumptionTariffIntervals*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ConsumptionTariffInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *EnvironmentalCosts*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *EnvironmentalCost*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *amount*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *costKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *costLevel*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numCostLevels*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *price*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *priceRatio*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *startValue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### RateComponentList  
<p>A List element to hold RateComponent objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|RateComponents|Array *RateComponents*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *RateComponent*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *roleFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveTimeTariffIntervalListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingTypeLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *TimeTariffIntervalListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### TariffProfileList  
<p>A List element to hold TariffProfile objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|TariffProfiles|Array *TariffProfiles*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *TariffProfile*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currency*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *pricePowerOfTenMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *primacy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *rateCode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *serviceCategoryKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *RateComponentListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### TimeTariffIntervalList  
<p>A List element to hold TimeTariffInterval objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|TimeTariffIntervals|Array *TimeTariffIntervals*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *TimeTariffInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeStart*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ConsumptionTariffIntervalListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### MessagingProgramList  
<p>A List element to hold MessagingProgram objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|MessagingPrograms|Array *MessagingPrograms*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *MessagingProgram*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *locale*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *primacy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveTextMessageListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *TextMessageListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### TextMessageList  
<p>A List element to hold TextMessage objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|TextMessages|Array *TextMessages*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *TextMessage*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *originator*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *priority*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *textMessage*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### BillingPeriodList  
<p>A List element to hold BillingPeriod objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|BillingPeriods|Array *BillingPeriods*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *BillingPeriod*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *billLastPeriod*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *billToDate*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *statusTimeStamp*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### BillingReadingList  
<p>A List element to hold BillingReading objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|BillingReadings|Array *BillingReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *BillingReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Charges*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Charge*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *kind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### BillingReadingSetList  
<p>A List element to hold BillingReadingSet objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|BillingReadingSets|Array *BillingReadingSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *BillingReadingSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *BillingReadingListLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### CustomerAccountList  
<p>A List element to hold CustomerAccount objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|CustomerAccounts|Array *CustomerAccounts*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *CustomerAccount*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currency*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *customerAccount*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *customerName*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *pricePowerOfTenMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *CustomerAgreementListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ServiceSupplierLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### CustomerAgreementList  
<p>A List element to hold CustomerAgreement objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|CustomerAgreements|Array *CustomerAgreements*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *CustomerAgreement*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *serviceAccount*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *serviceLocation*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveBillingPeriodListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveProjectionReadingListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveTargetReadingListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *BillingPeriodListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *HistoricalReadingListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PrepaymentLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ProjectionReadingListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *TargetReadingListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *TariffProfileLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *UsagePointLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### HistoricalReadingList  
<p>A List element to hold HistoricalReading objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|HistoricalReadings|Array *HistoricalReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *HistoricalReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *BillingReadingSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingTypeLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ProjectionReadingList  
<p>A List element to hold ProjectionReading objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|ProjectionReadings|Array *ProjectionReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *ProjectionReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *BillingReadingSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingTypeLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### TargetReadingList  
<p>A List element to hold TargetReading objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|TargetReadings|Array *TargetReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *TargetReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *BillingReadingSetListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ReadingTypeLink*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### ServiceSupplier  
<p>Organisation that provides services to Customers.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|email|string *email*|Yes|Yes|Yes|Yes| |
|phone|string *phone*|Yes|Yes|Yes|Yes| |
|providerID|integer *providerID*|Yes|Yes|Yes|Yes| |
|web|string *web*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |
|mRID|array *mRID*|No|Yes|Yes|Yes| |
|description|string *description*|Yes|Yes|Yes|Yes| |
|version|integer *version*|Yes|Yes|Yes|Yes| |


##### AccountBalance  
<p>AccountBalance contains the regular credit and emergency credit balance for this given service or commodity prepay instance. It may also contain status information concerning the balance data.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|availableCredit|Struct *availableCredit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|No|Yes|Yes|Yes| |
|creditStatus|integer *creditStatus*|Yes|Yes|Yes|Yes| |
|emergencyCredit|Struct *emergencyCredit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|emergencyCreditStatus|integer *emergencyCreditStatus*|Yes|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### CreditRegisterList  
<p>A List element to hold CreditRegister objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteCreditRegister|href:&nbsp;string *href* |Yes| |
|None|CreateCreditRegister|CreditRegister:&nbsp;Struct *CreditRegister*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *AccountingUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *creditType*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *effectiveTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *token*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|CreditRegisters|Array *CreditRegisters*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *CreditRegister*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *AccountingUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creditType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *effectiveTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *token*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PrepaymentList  
<p>A List element to hold Prepayment objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteUsagePoint|href:&nbsp;string *href* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|Prepayments|Array *Prepayments*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *Prepayment*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *AccountingUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *AccountingUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *AccountingUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *monetaryUnit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *prepayMode*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *UsagePoints*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *UsagePoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *roleFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *serviceCategoryKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *MeterReadingListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *AccountBalanceLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveCreditRegisterListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveSupplyInterruptionOverrideListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *CreditRegisterListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *PrepayOperationStatusLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *SupplyInterruptionOverrideListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *UsagePointLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### PrepayOperationStatus  
<p>PrepayOperationStatus describes the status of the service or commodity being conditionally controlled by the Prepayment function set.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|creditTypeChange|Struct *creditTypeChange*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *newType*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *startTime*|Yes|Yes|Yes|Yes| |
|creditTypeInUse|integer *creditTypeInUse*|Yes|Yes|Yes|Yes| |
|serviceChange|Struct *serviceChange*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *newStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *startTime*|Yes|Yes|Yes|Yes| |
|serviceStatus|integer *serviceStatus*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### SupplyInterruptionOverrideList  
<p>A List element to hold SupplyInterruptionOverride objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|SupplyInterruptionOverrides|Array *SupplyInterruptionOverrides*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *SupplyInterruptionOverride*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### FlowReservationRequestList  
<p>A List element to hold FlowReservationRequest objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteFlowReservationRequest|href:&nbsp;string *href* |Yes| |
|None|CreateFlowReservationRequest|FlowReservationRequest:&nbsp;Struct *FlowReservationRequest*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *durationRequested*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *SignedRealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RequestStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *requestStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|FlowReservationRequests|Array *FlowReservationRequests*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *FlowReservationRequest*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *durationRequested*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *SignedRealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RequestStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *requestStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### FlowReservationResponseList  
<p>A List element to hold FlowReservationResponse objects.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|FlowReservationResponses|Array *FlowReservationResponses*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *FlowReservationResponse*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *RealEnergy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ActivePower*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *subject*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DefaultDERControl  
<p>Contains control mode information to be used if no active DERControl is found.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|DERControlBase|Struct *DERControlBase*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *opModFixedFlow*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *FixedPowerFactor*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *displacement*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *FixedVAr*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *refType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *opModFixedW*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *CurvePairType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *CurvePairType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampTms*|No|Yes|Yes|Yes| |
|mRID|array *mRID*|No|Yes|Yes|Yes| |
|description|string *description*|Yes|Yes|Yes|Yes| |
|version|integer *version*|Yes|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERList  
<p>A List element to hold DER objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteDER|href:&nbsp;string *href* |Yes| |
|None|CreateDER|DER:&nbsp;Struct *DER*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *AssociatedDERProgramListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *AssociatedUsagePointLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *CurrentDERProgramLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERAvailabilityLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERCapabilityLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERSettingsLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERStatusLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|DERs|Array *DERs*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *DER*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *AssociatedDERProgramListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *AssociatedUsagePointLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *CurrentDERProgramLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERAvailabilityLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERCapabilityLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERSettingsLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERStatusLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERSettings  
<p>Distributed energy resource settings</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|setGenConnect|boolean *setGenConnect*|Yes|Yes|Yes|Yes| |
|setGradW|integer *setGradW*|No|Yes|Yes|Yes| |
|setMaxChargeRate|Struct *setMaxChargeRate*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setMaxDischargeRate|Struct *setMaxDischargeRate*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setMaxVA|Struct *setMaxVA*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setMaxVAr|Struct *setMaxVAr*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setMaxVArNeg|Struct *setMaxVArNeg*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setMaxW|Struct *setMaxW*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|No|Yes|Yes|Yes| |
|setMinPF|Struct *setMinPF*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setMinPFNeg|Struct *setMinPFNeg*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setStorConnect|boolean *setStorConnect*|Yes|Yes|Yes|Yes| |
|setVRef|Struct *setVRef*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|setVRefOfs|Struct *setVRefOfs*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|updatedTime|integer *updatedTime*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERAvailability  
<p>Indicates current reserve generation status</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|availabilityDuration|integer *availabilityDuration*|Yes|Yes|Yes|Yes| |
|maxChargeDuration|integer *maxChargeDuration*|Yes|Yes|Yes|Yes| |
|readingTime|integer *readingTime*|No|Yes|Yes|Yes| |
|reserveChargePercent|integer *reserveChargePercent*|Yes|Yes|Yes|Yes| |
|reservePercent|integer *reservePercent*|Yes|Yes|Yes|Yes| |
|statVArAvail|Struct *statVArAvail*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|statWAvail|Struct *statWAvail*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERCapability  
<p>Distributed energy resource type and nameplate ratings.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|modesSupported|array *modesSupported*|No|Yes|Yes|Yes| |
|rtgA|Struct *rtgA*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|No|Yes|Yes|Yes| |
|rtgAh|Struct *rtgAh*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgMaxChargeRate|Struct *rtgMaxChargeRate*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgMaxDischargeRate|Struct *rtgMaxDischargeRate*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgMinPF|Struct *rtgMinPF*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgMinPFNeg|Struct *rtgMinPFNeg*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgVA|Struct *rtgVA*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgVAr|Struct *rtgVAr*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgVArNeg|Struct *rtgVArNeg*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|rtgW|Struct *rtgW*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|No|Yes|Yes|Yes| |
|rtgWh|Struct *rtgWh*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|type|integer *type*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERControlList  
<p>A List element to hold DERControl objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteDERControl|href:&nbsp;string *href* |Yes| |
|None|CreateDERControl|DERControl:&nbsp;Struct *DERControl*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERControlBase*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *opModFixedFlow*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *FixedPowerFactor*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *displacement*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *FixedVAr*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *refType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *opModFixedW*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *CurvePairType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *CurvePairType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampTms*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeStart*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|DERControls|Array *DERControls*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *DERControl*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERControlBase*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *opModFixedFlow*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *FixedPowerFactor*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *displacement*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *FixedVAr*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *refType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *opModFixedW*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *CurvePairType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *CurvePairType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DERCurveLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampTms*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *EventStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *currentStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *potentiallySuperseded*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *potentiallySupersededTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *reason*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *responseRequired*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *replyTo*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeDuration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *randomizeStart*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERCurveList  
<p>A List element to hold DERCurve objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteDERCurve|href:&nbsp;string *href* |Yes| |
|None|CreateDERCurve|DERCurve:&nbsp;Struct *DERCurve*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Array *CurveDatas*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *CurveData*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *excitation*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *xvalue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *yvalue*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *curveType*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampDecTms*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampIncTms*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampPT1Tms*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *xMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *yMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *yRefType*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|DERCurves|Array *DERCurves*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *DERCurve*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *creationTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *CurveDatas*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *CurveData*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *excitation*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *xvalue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *yvalue*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *curveType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampDecTms*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampIncTms*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *rampPT1Tms*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *xMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *yMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *yRefType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*|Yes|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERProgramList  
<p>A List element to hold DERProgram objects.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|DeleteDERProgram|href:&nbsp;string *href* |Yes| |
|None|CreateDERProgram|DERProgram:&nbsp;Struct *DERProgram*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *primacy*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveDERControlListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DefaultDERControlLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERControlListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERCurveListLink* |Yes| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|DERPrograms|Array *DERPrograms*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *DERProgram*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *primacy*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *ActiveDERControlListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DefaultDERControlLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERControlListLink*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- uri *DERCurveListLink*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### DERStatus  
<p>DER status information.</p>


###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|genConnectStatus|Struct *genConnectStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|inverterStatus|Struct *inverterStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|localControlModeStatus|Struct *localControlModeStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|manufacturerStatus|Struct *manufacturerStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *value*|Yes|Yes|Yes|Yes| |
|operationalModeStatus|Struct *operationalModeStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|readingTime|integer *readingTime*|No|Yes|Yes|Yes| |
|stateOfChargeStatus|Struct *stateOfChargeStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|storageModeStatus|Struct *storageModeStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|storConnectStatus|Struct *storConnectStatus*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *dateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*|Yes|Yes|Yes|Yes| |
|subscribable|integer *subscribable*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |


##### MirrorUsagePointList  
<p>A List of MirrorUsagePoint instances.</p>


###### Actions
|Return Type |Name |Arguments |Optional |Documentation |
|:-----------|:----|:---------|:--------|:-------------|
|None|CreateMirrorMeterReading|MirrorMeterReading:&nbsp;Struct *MirrorMeterReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastUpdateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Array *MirrorReadingSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *MirrorReadingSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Readings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *nextUpdateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ReadingType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *accumulationBehaviour*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *commodity*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dataQualifier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *flowDirection*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *intervalLength*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *kind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxNumberOfIntervals*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numberOfConsumptionBlocks*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numberOfTouTiers*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *phase*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *powerOfTenMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subIntervalLength*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyDisconnectLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyWarningLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *tieredConsumptionBlocks*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *uom*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version* |No| |
|None|DeleteMirrorUsagePoint|href:&nbsp;string *href* |No| |
|None|DeleteReading|href:&nbsp;string *href* |Yes| |
|None|CreateMirrorUsagePoint|MirrorUsagePoint:&nbsp;Struct *MirrorUsagePoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *deviceLFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;- Array *MirrorMeterReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *MirrorMeterReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastUpdateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *MirrorReadingSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *MirrorReadingSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Readings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *nextUpdateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ReadingType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *accumulationBehaviour*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *commodity*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dataQualifier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *flowDirection*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *intervalLength*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *kind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxNumberOfIntervals*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numberOfConsumptionBlocks*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numberOfTouTiers*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *phase*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *powerOfTenMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subIntervalLength*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyDisconnectLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyWarningLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *tieredConsumptionBlocks*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *uom*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *roleFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *serviceCategoryKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;- integer *version* |No| |

###### Data
|Name |Type |Optional |Writable |Readable |Eventable |Documentation |
|:----|:----|:--------|:--------|:--------|:---------|:-------------|
|MirrorUsagePoints|Array *MirrorUsagePoints*: <br />&nbsp;&nbsp;&nbsp;&nbsp;Struct *MirrorUsagePoint*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *deviceLFDI*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *MirrorMeterReadings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *MirrorMeterReading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *lastUpdateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *MirrorReadingSets*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *MirrorReadingSet*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Array *Readings*: <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *nextUpdateTime*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *Reading*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *localID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subscribable*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *consumptionBlock*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *qualityFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *DateTimeInterval*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *duration*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *start*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *touTier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *ReadingType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *accumulationBehaviour*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *commodity*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Struct *UnitValueType*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *multiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *unit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *value*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *dataQualifier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *flowDirection*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *intervalLength*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *kind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *maxNumberOfIntervals*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numberOfConsumptionBlocks*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *numberOfTouTiers*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *phase*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *powerOfTenMultiplier*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *subIntervalLength*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyDisconnectLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *supplyWarningLimit*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- boolean *tieredConsumptionBlocks*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *uom*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *href*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *roleFlags*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *serviceCategoryKind*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *status*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- array *mRID*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- string *description*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- integer *version*|Yes|Yes|Yes|Yes| |
|all|integer *all*|No|Yes|Yes|Yes| |
|results|integer *results*|No|Yes|Yes|Yes| |
|href|string *href*|No|Yes|Yes|Yes| |