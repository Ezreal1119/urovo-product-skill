# RFG91 UHF RFID Sled User Manual

> **Canonical original:** `RFG91/user_guide/default_202608151705/RFG91-User_Manual_20251215.pdf`
> **Document date:** 2025-12-15 (from the source filename); revision V2.1 (2025/12/11)
> **Language:** English
> **Publisher:** UROVO PTE. LIMITED
> **Scope note:** The RFG91 is a handheld UHF RFID sled that holds a DT610 (or DT610 Pro) mobile computer. It comes in Bluetooth and Pogo-pin wired versions.

> **Repair coverage:** Complete page-by-page transcription of all 39 source pages. Native PDF text is preserved in page order. Every page was also rendered and checked with OCR; high-confidence text from image-dominant pages is listed separately on its source page.

## Complete Page-by-Page Transcription

### Page 1

```text
RFG91    User  Manual

                                      V2.1

            UROVOPTE.LIMITED
```

### Page 2

```text
Copyright Statement

               ThisdocumentisthepropertyofUROVOPTE.LIMITED.

               Nopartofthisdocumentmaybereproduced,disclosed,ordistributedtoanythirdparty
            withoutthepriorwrittenconsentofUROVOPTE.LIMITED.Anyunauthorizedusewillbe

            subjecttolegalaction.

               ThisdocumentservesastheusermanualfortheRFG91product.Theactualoperation

            mayvarydependingonthefunctionsofthecustomer’shandhelddevice.Pleasereadthis

            manualcarefullybeforeuseandoperateinaccordancewiththeprovidedinstructionsto
            ensureproperandsafeusage.

            Safety Precautions

               Topreventinjuryordamage,pleasereadthismanualcarefullybeforeusingthedeviceto
            ensureproperandsafeoperation.

               Onlyuseaccessoriesapprovedbythemanufacturerandspecificallydesignedforthis

            devicemodel.Theuseofunauthorizedpoweradapters,chargers,orbatteriesmayresultin

            fire,explosion,orotherhazards.

               Operatethedeviceonlywithinthespecifiedtemperaturerange.Extremelyhighorlow

            environmentaltemperaturesmaycausemalfunctionorpermanentdamage.
               Donotdisassembleormodifythedeviceoritsaccessories.Ifthedeviceorany

            componentfailstofunctionproperly,contactafter-salessupportortakethedevicetoan

            authorizedservicecenterforinspectionandrepair.

               Batteriesareflammableandmayexplodeifmishandled.Donotdisassemble,crush,

            puncture,orexposethebatterytohightemperatures.

               Disposeofusedbatteriesinaccordancewithlocallawsandregulationsorfollowlocal
            batteryrecyclingpolicies.
```

### Page 3

```text
Revision History

             Version   Date    AMD       Reviser        Description

               V1.0  2025/07/01 A        Wayne       Initialversion

               V1.1  2025/10/23 M         蒋豪      Modifiedthepagelayout.

                                                  Contentrestructured,newdemo

               V2.0  2025/10/23 A/M/D    NolanLo  replaced,additionalinformation
                                                  added,anddescriptionsre-edited.

                                                  Contentrestructured,newdemo

                                                  replaced,additionalinformation
              V2.1   2025/12/11 A/M/D   HanCheng
                                                  added,andoptionalaccessory

                                                  added.

            (A-Add,M-Modify, D-Delete)
```

### Page 4

```text
Contents

            RFGS91UserManual.............................................................................................................................1

               CopyrightStatement..........................................................................................................................2
               SafetyPrecautions.............................................................................................................................2

            1.AppearanceOverview.....................................................................................................................1

               1.1WirelessBluetoothversion..........................................................................................................1

                  1.1.1Overview..........................................................................................................................1

                  1.1.2BatteryInstallationandRemoval.....................................................................................2

               1.2PogopinWiredversion...............................................................................................................4

            2. FunctionDescription....................................................................................................................6

               2.1KeyDefinition.............................................................................................................................6
               2.2IndicatorInstructions...................................................................................................................7

               2.3BuzzerandStandbyInteractionInstructions...............................................................................7

                  2.3.1BuzzerDescription...........................................................................................................7

                  2.3.2AudioandStandbyInteraction.........................................................................................8

            3.ConnectRFIDModule....................................................................................................................9

               3.1ConnectingtheBluetoothVersionoftheRFG91RFIDHandle................................................9

               3.2ConnectingthePogoVersionoftheRFG91RFIDHandle......................................................10

               3.3Built-inShortRangeRFIDmodule...........................................................................................11
            4.CoreSoftwareFunctionModule................................................................................................11

               4.1TagInventory(Scan).................................................................................................................13

               4.2TagManagement.......................................................................................................................15

               4.3TagFinder(Location)................................................................................................................17

               4.4SceneMode(Profiles)...............................................................................................................17

               4.5BasicSettings............................................................................................................................20

               4.6Filter..........................................................................................................................................22

               4.7DataOutput...............................................................................................................................24
               4.8InventoryLEDScreenDescription...........................................................................................24
```

### Page 5

```text
4.9RFIDSled..................................................................................................................................25

            5.OptionalAccessory.......................................................................................................................26

            6.FAQ....................................................................................................................................................27

               6.1ConnectionIssues......................................................................................................................27

               6.2Reading/TagDetectionIssues...........................................................................................28

               6.3ApplicationFunctionIssues..................................................................................................29
               6.4PerformanceandDisplaysIssues.......................................................................................29

               6.5HardwareIssues....................................................................................................................30

            7.ErrorCodeandTroubleshootingGuide.................................................................................30

               7.1ErrorCodeTable.......................................................................................................................30

               7.2TroubleshootingProcedure.......................................................................................................34

            8.CareandMaintenance..................................................................................................................34
```

### Page 6

```text
1. Appearance Overview

            1.1 Wireless Bluetooth version

            1.1.1Overview

                                         1
```

#### Visual Text Recovered From Page Imagery

- Battery LED
- Bluetooth LED
- Mode LED
- Decode status LED
- Battery switch

### Page 7

```text
1.1.2BatteryInstallationandRemoval

            InstallingtheBattery

                                         2
```

#### Visual Text Recovered From Page Imagery

- BT mode Button
- Mode switch Button
- Power Button
- NFC touch area for Bluetooth connection
- Hand strap hole

### Page 8

```text
RemovingtheBattery:

                                         3
```

#### Visual Text Recovered From Page Imagery

- Press the battery release buttons on the
- lower part of the handle and pull the
- battery out.

### Page 9

```text
1.2 Pogo pin Wired version

            Note:thepogoversiondoesnotcontaintheBluetoothfeatureandScanenginebydefault.The

               BluetoothbuttonandModebuttonwillbedisabled.

            1.2.1InstallationInstructions
            Step1. InstalltheBatteryandPowerOn

               RemovetheRFIDsledfromthepackageandinstallthebatteryproperly.

               PressandholdthePowerKeytoturnontheRFIDsled.

            Step2. AligntheDT610withtheRFIDHandle

               PlacetheDT610devicefaceup,alignthetopofthedevicewiththefrontslotoftheRFIDhandle,

            andinsertitcarefully.

                                         4
```

### Page 10

```text
Step3. SecuretheDevice

               PressdownontherearendoftheDT610untilthedeviceisfullyseatedandlockedintothehandle

            slot.

              Note:Ensurethatthepogo-pinconnectorsbetweentheDT610andtheRFIDhandlearecleanand
            ⚠
            alignedbeforeinstallationtoavoidconnectionfailure.

                                         5
```

### Page 11

```text
2.  Function Description

            2.1 Key Definition

                 PhysicalKey       Action              Function

                             Longpressfor2seconds Turnon/offthedevice

                                              Powerindicatorlightsfor1second:

             PowerButton     Shortpresswhenpowered red(1%–20%),

                             on               yellow(21%–70%),

                                              green(71%–100%)

             ModeButton
                             Longpressfor1second SwitchbetweenRFID/SCANmodes
             (onlyBluetoothversion)

                             Longpressfor3seconds
                                              Forceenterpairingmode
             BluetoothButton whenpoweredon
             (onlyBluetoothversion) Longpressfor3seconds Forceexitofflinemodeandenterpairing

                             inofflinemode    mode

                             Press/ReleaseinRFID
                                              Trigger/InterrupttheRFIDreading
                             mode

                             Press/ReleaseinSCAN Trigger/Interruptthescanningand

                             mode             decoding

                             Longpressthetriggerkey Enterfirmwaredownloadmode:

             TriggerKey      andpowerbutton   Thepowerindicatorflashesgreenandred

                             simultaneouslyfor3 alternatelyfor1second,whilethebuzzer
                             secondswhenpoweredoff beeps5shorttimes.

                                              Activatethedevice:

                             Pressinsleepmode TheBluetoothindicatorstayson,while

                                              thebuzzerbeeps2shorttimes.

                                         6
```

### Page 12

```text
2.2 Indicator Instructions

               LEDIndicator   CorrespondingDeviceState   LightStatus

             DecodingLight SuccessfulSCAN/RFIDread Greenlightflashes

                           CriticalLowPower(<10%)  Redlightflashesbriefly

                           LowPowerwarning(=20%)   Redlightflashes

                           Charging(whenbatterylevel<20%) Redlightstayson

                           Charging(whenbatterylevel21%
                                                   Yellowlightstayson
             PowerIndicator –70%)

                           Charging(whenbatterylevel71%
                                                   Greenlightflashes
                           –99%）

                           Charging(afteralmostfullcharge,
                                                   Greenlightstayson
                           batterylevel95%–100%)

                           Bluetoothconnected      Bluelightstayson
             BluetoothLight
                           Connecting              Bluelightflashesrapidly
             (onlyBluetooth
                           Disconnected/searchable Bluelightflashes
             version)
                           Offline                 Nolight

             ModeLight     RFIDreading             Greenlightstayson

             (onlyBluetooth Longpresstoswitchtoscanengine Nolight
             version)      RFIDandScanactivesimultaneously Yellowlightstayson

            2.3 Buzzer and Standby Interaction Instructions

            2.3.1BuzzerDescription

               Thissectiondescribesthebuzzerbehaviorunderdifferentpower,scan,andstatusconditions.

                  Condition     Trigger      BuzzerBehaviorDescription

            PowerOn            Power   Soundthreeascending-volumebeeps

            PowerOff           Power   Soundthreedescending-volumebeeps

            CriticalLowPower(<10%) Power Threelow-frequencyshortbeeps,singlealertonly.

                                         7
```

### Page 13

```text
Condition     Trigger      BuzzerBehaviorDescription

            LowPower(<20%)     Power   Twolow-frequencyshortbeeps

            Charging           Power   Singleshortbeep

            FullyCharged       Power   Highestpitch,shortbeeponce.

            SuccessfulRFIDTagRead RFID Beepfrequencyanddurationvarybasedontagread

                                       speed;repeatedreadstriggershorterintervals.

            SuccessfulBarcodeRead Scan Singleshortbeep.

            OfflineScan        Scan    Successfulreadsareconfirmedbythreeshortbeeps

            DeviceQueryorSetup Status  Singlebeeptoacknowledgeaction.

            ModeSwitch         Status  Singlebeeptoindicatemodechange.

            (onlyBluetoothversion)

            BluetoothDisconnectionor Status Twoshortbeepstoindicatestatustransition.

            Reconnection

            (onlyBluetoothversion)

            2.3.2AudioandStandbyInteraction

               Thissectionexplainstimeoutandvolumeinteractionsettingsduringstandbyandoperation.

                 Item        DefaultSetting  Description AdjustableRange

            AutoPower-off Default:60×10s  Devicepowersoff Adjustable:N×10s
            Timeout                       automaticallywitha

                                          buzzeralert.

            SleepTimeout  Default:6×10s   Indicatorlightturnsoff Adjustable:N×10s

                                          anddeviceenterssleep

                                          mode.

            BuzzerVolume  Default:10      Adjustablebuzzer Range:0–10

                                          volume.

                                         8
```

### Page 14

```text
3 . Connect RFID Module

                                         TheAndroidversionisgenerallyprovidedwith
                                      abuilt-insystemapplicationnamedRFIDDemo.

                                        IfyourequireotherplatformssuchasiOSor

                                      Windows,pleasecontactUrovotechnicalsupport

                                      forassistance.

                                      Note:Bydefault,thesystemselectstheBatteryLife

                                      (PowerOptimization)modetoreducepower
                                      consumptionunderthecurrentreadconfiguration.

                                        Theactualtransmitpower(dBm)maybelimiteddue

            toregionalregulatoryrequirements.

            3.1 Connecting the Bluetooth Version of the RFG91 RFID Handle

                                         9
```

### Page 15

```text
• MakesuretheRFG91handleispoweredon,whiletheBluetoothofboththeRFG91handle

            andPDAalsomustbeactive.

            • LocateandopentheRFIDDemoapplicationonthedesktop.

            • Click“WirelessConnection”.
            • Choosepairingmethodsasfollow:

            1) CameraScanning(scantheQRcodeofRFG91)

            2) ManualSearch(searchtheBLEofRFG91)

            3) NFCpairing

                For example, while DT610 is pairing with RFG91, please tap the under-display area of

            DT610totheNFCzoneonthebackofRFG91RFIDmodule.

            • Oncetheconnectionissuccessful,thesystemwillautomaticallyentertheScanPagefor

            inventory.

            3.2 Connecting the Pogo Version of the RFG91 RFID Handle
            • MakesuretheRFG91handleispoweredon.

                                        10
```

### Page 16

```text
• EnsuretheRFG91handleandtheDT610

                                       devicearefirmlyandfullyconnected.

                                       • LocateandopentheRFIDDemoapplication

                                       onthedesktop.
                                       • Click“WiredConnection”.

                                       • EntertheScanPagetostartinventory.

                                       Note:WhilethePogoversionofRFG91ina

                                       power-offstateisconnectedwithDT610,

                                       clicking“WiredConnection”willbringaprompt
                                       indicatingthatinitializationhasfailed，shownas

                                       follow.

            3.3 Built-in Short Range RFID module

            1.MakesuretheexternalRFIDhandleRFG91isneitherconnectedviapogopinnor
            Bluetooth;

            2.LocateandopentheRFIDDemoapplicationonthedesktop;

            3.Click“WiredConnection”;

            4.EntertheScanpagetostartinventory.

            4. Core Software Function Module

               ThissectionprovidesanoverviewofthemainfeaturesandfunctionsoftheRFIDDemo

            application.

               TheapplicationisdesignedtosupporttheRFIDreading,writing,andtagmanagement

            capabilitiesofUrovodevicesorexternalRFIDhandlessuchastheRFG91.

                Bar    MainFunctionModule      DetailedDescription

                       TagInventory(Scan) ExecutesRFIDtagreadingandpresentstheamount

                                      ofuniquetagsandtotalreads(cumulativeread
            NavigationBar
                                      quantity)duringthescanningprocess.

                       TagManagement  Performsread,write,lockorkilloperationson

                                        11
```

### Page 17

```text
Bar    MainFunctionModule      DetailedDescription

                                      individualRFIDtagretrievedfromthedetectedtag

                                      list.

                       TagFinder(Location) Enablesreal-timesignalintensitytolocateaspecific

                                      targetRFIDtag.

              SlideBar SceneMode(Profiles) Thedefaultoperationalsettingis“PowerSaving”

                                      mode,whichprioritizespowerconservationfor
                                      extendeddeviceruntime.

                                      Userscanalsoswitchtoalternativemodesincluding

                                      “FullInventory”,“RapidRepeat”,“Balanced

                                      Performance”,“CycleCount”,“MaxRange”,

                                      “Custommode”,eachofwhichisconfiguredwith

                                      differentparameterstomeetwithvariousperformance
                                      requirements.

                       BasicSettings  Allowsuserstoadjustmaindeviceparameters,

                                      includingRFoutputpowerlevel,RFspectrum,tag

                                      focusandinventorybank.

                       Filter         Servesasatagdatafilteringtoolsthatsupportsboth

                                      flexiblematchingandexactmatching.

                                      Onceafilterruleisapplied,thescanpagecanbe
                                      customizedtoeitherdisplayonlythetagsthatmeet

                                      thefiltercriteriaorexcludenon-complianttagsfrom

                                      thetaglist.

                       Dataoutput     Allowsuserstoexportallthedetectedtags.

                       LEDTagDemonstration DesignedfordetectingtheLED-integratedRFIDtags

                       （InventoryLed） andperformingcertaintaginventory,whichactivate

                                      theLEDlightofRFIDtagsthroughRF
                                      communication.

                                        12
```

### Page 18

```text
Bar    MainFunctionModule      DetailedDescription

                       RFIDSled       DeliversanoverviewofRFG91basicoperational

                                      status,whileenablinguserstoconfiguretimeout

                                      thresholdsandbuzzerparameters.Itactsasacontrol

                                      paneltocheckdeviceSN,RFIDfirmwareversionand

                                      BLEprotocolversion.

            4.1 TagInventory(Scan)

               ThisscreenisusedtoperformfastRFIDtaginventoryoperations,resultinginreal-timestatistics.

            Itallowsuserstoquicklymeasuretagperformanceandreadingstabilityunderdifferentenvironments

            andpowersettings.

                                        13
```

### Page 19

```text
FunctionItem                BriefDescription

            [1]Single/CycleMode Providestwoscanningmodeoptionsforuserstoselect:singlescan

                           (one-timereading)orcontinuousreading(cyclescanning).

            [2]UniqueTags  Displaysthecountofnon-repetitivetagsdetectedduringthecurrent

                           scanningprocess.

            [3]ReadRate(Pcs/sec) Indicatesthetagreadingspeed,specificallyshowingthenumberoftags
                           readpersecond.

            [4]TotalReads  Showsthecumulativenumberoftagsreadincludingrepeatedreadsofthe

                           sametag.

            [5]ReadTime    Displaysthetotaldurationoftheongoingscanningsession.

            [6]ASCII       Afunctionalswitch;whenenabled,tagdatawillbedisplayedinASCII

                           formatinreplaceofthedefaulthexadecimalformat.

            [7]START       Clicksthisbuttontoinitiatetaginventory.

            SCANNING       Inthemodeofcyclereading,iftheRFIDreaderisactivatedbyits

                           physicaltrigger,theon-screenbuttonsautomaticallysynchronizewiththe
                           physicaltrigger,meaningthattheRFIDreadingstartsorstopsasthe

                           triggerispressedorreleased.

            [8]CLEAR       Enablestoclearallcurrenttagreadingresultsfromthedisplaylist.

            [9]TagListArea Servesasthededicateddisplayareafortaginformation,showingthree
            (EPC/COUNT/RSSI) keyparametersforeachdetectedtag:

                           •ElectronicProductCodeofthetag

                           •Thenumberoftimesthetaghasbeendetected

                           •Signalstrengthindicatorofthetag

                                        14
```

### Page 20

```text
4.2 Tag Management

               ThisfunctionisdesignedformanagingindividualRFIDtags,whichallowsuserstoselectonetag

            fromtheScanpageandthenproceedtotheTagManagementpageforfurtheraction.Herearethree

            mainfunctionaltabsasfollow.Itisidealforadvancedtagmanagementscenariossuchasdata
            protection,inventorycontrolorsecuretagdeactivationduringdevicelifecyclemanagement.

                FunctionBar    Step              SpecificAction

                            SelectTag  Selectaspecifictagfromthelist.

                            MemoryBank Choosethememorybank,includingEPC,TID,

                                       USER,AccessPassword.

               Read/Writetag Password  Enterthetag’saccesspassword(default:00000000)

            (usedforreadingor StartingAddress Definetheaddressoffsetanddatalengthfor

            writingtagdatain /DataLength read/writeoperations.
            differentmemoryareas)      Note:PCselectiondeterminesthelengthandformat

                                       ofthetagEPCmemoryarea.

                            LabelData  Inputordisplaythetagdata,whichsupportsHEXor

                                       ASCIIformat.

                                        15
```

### Page 21

```text
FunctionBar    Step              SpecificAction

                            READTAG    Executereadorwriteoperationsontheselectedtag.

                            /WRITETAG

                 LockTag    StorageArea Choosethememoryareatolock,includingdestroy

            (usedforlockingspecific    oraccesspassword,EPC,TID,USER.

            memoryareastoprevent Password Enterthecurrentaccesspassword.

            unauthorizedchanges)

                            LockMode   Selectfromopen,close,permanentopenor

                                       permanentclose.

                                       Note:tagscan’tbeunlockedafterpermanentlock.

                            LOCKED     Executethelockcommand.

                 KillTag    SelectTag  Selectaspecifictagfromthelist.
            (usedforpermanently KillPassword Entertherequiredpasswordtoexecutethekill

            disablingaRFIDtag)         command.

                            DESTROY    Permanentlyinvalidatetheselectedtag,whichcan

                                       notbereadorwrittenanymore.

                                        16
```

### Page 22

```text
4.3 Tag Finder (Location)

               ThisscreenhelpuseslocateaspecificRFIDtagby

            continuouslymeasuringanddisplayingitsreal-time

            signalstrength(RSSI).Userscantrackproximity
            changestodeterminethetag’sposition,makingit

            especiallyusefulforretrievingitems,locatingassetsor

            verifyingtagpresence.

            Thisfeatureallowsquickandaccurateidentificationof

            atargettageveninenvironmentswithmultipleRFID

            tagspresent.

                  Step                     BriefDescription

             [1]SelectTag  ChoosetheEPCofthetagtobelocated

             [2]SignalIntensity Displaythereal-timesignalstrengthofthetargettag.
                           Thiscircularprogressbarprovidesavisualrepresentationofsignal

                           strength.Oncemoveclosertothetag,thegreenarcofthegaugeexpands.

             [3]PauseButton Temporarilypausesthetagsearchingprocess.Clickthebuttonagainor

                           pressthetriggerontheRFG91handletoresumetaglocating.

            4.4 Scene Mode (Profiles)

               ThisscreenallowsuserstoselecttheRFIDreader’sperformancemodetoadjustperformanceand
            powerconsumptionaccordingtopracticalneeds.Userscanopenthesidebarbyswipingrightfromthe

            leftedgeofthescreen.HereistheProfilesasbelow.

                                        17
```

### Page 23

```text
Operating   MainFunction    KeyFeaturesandApplicableScenarios

                Mode

             PowerSaving Optimizesformaximum •Reducestransmissionpowerandreading

             (Defaultmode) batteryefficiency. frequencytoextendoperatingtime.

                                        •Recommendedforcontinuousfielduse.

             FullInventory Readsallavailabletagsas •SuitableformostgeneralRFIDinventory

                        quicklyaspossiblewith scenarios.

                        stableandconsistent •OffersbalancedperformancebetweenRapidand

                        performance.    Cyclemodes.

             RapidRepeat Quicklyinventoriesand •SuitablefordemonstratingRFIDreadingspeed.

                        accumulatesnearbytags, •Providesfasterbutlesscomprehensivetag

                        withduplicatetagcounts coveragecomprehensiveness.

                        increasingrapidly.

                                        18
```

### Page 24

```text
Operating   MainFunction    KeyFeaturesandApplicableScenarios

                Mode

             Balanced   BalancesRFIDreading •ProvidesmoderateRFpoweroutputandtag

             Performance performanceanddevice readingrate.

                        batterylife.    •Recommendedfordailyoperationwhereboth

                                        batteryenduranceandreadingresponsivenessare

                                        required.

             CycleCount Inventoriesallavailable •Readingspeeddecreasesinsubsequentscans

                        tagswithoutduplicate afteralltagsaredetectedforthefirsttime.

                        counts,ensuring •Suitableforhigh-interferenceenvironmentsor

                        comprehensivetag scenarioswithdensetagdeployment.
                        coverage.

             MaxRange   Optimizesfor    •Prioritizesreadingdistanceoverreadingspeed

                        long-distancesingletag and thequantityoftagsreadsimultaneously.

                        readingandperformance •Suitablefortestingthemaximumreadrange

                        evaluation.     underidealoperatingconditions.

             Custommode Allowscustomizationof •Providesflexibilityforadvancedusersto

                        keyparameterssuchasRF fine-tuneperformanceforspecificapplications.

                        power,readinginterval,or

                        sessionconfiguration,

                        whichareshowninabove
                        page.

                                        19
```

### Page 25

```text
4.5 Basic Settings

               Thisscreenprovidesessentialconfiguration

            optionsfortheRFIDreader,whichallowsusers

            tochangekeyhardwareparameterssuchasRF
            outputpower,frequencyband,andtagdata

            readingmode.ThesesettingshelpoptimizeRFID

            performanceinaccordingwithregional

            regulations,ambientenvironmentsandspecific

            applicationscenarios.

            EPCmodeandkeepingRFpoweroutputlevel
            between26–30dBmarerecommendedformost

            scenarios.However,itbecomesnecessaryto

            adjustspectrumandpowersettingswhen

            deployingacrossdifferentcountriesorunder

            specialinterferenceconditions.

                 Parameter             DescriptionsandSpecifications

              [1]FirmwareVersion •DisplaysthecurrentfirmwareversionoftheRFIDreader(e.g.,v2.15).
                            Version2andaboveisGen2xcompliant.

                            •Usedtoconfirmcompatibilitywiththedemoapplicationandconfirm

                            thedevicerunsthelatestfirmwarerelease.

              [2]RFOutputPower Adjuststhetransmissionpowerofthereader’santenna,measuredin

                            dBm.Higherpowerincreasesreaddistancebutincreasespower
                            consumption.

                            •Long-rangereaders:0–30dBm

                            •Short-rangereaders:0–26dBm

                            Note:TapSettingstoconfigurepowerorReadtocheckthecurrent

                                        20
```

### Page 26

```text
Parameter             DescriptionsandSpecifications

                            outputlevel.

              [3]RFSpectrum Selectstheregionalfrequencystandardincompliancewiththelocal

                            regulatoryrequirements.

                            •FCC:902–928MHz

                            •EU2:916-920MHz

                            •Chinese2:920-925MHz
                            •Taiwan(China):920-928MHz

                            •Japan:916-921MHz

                            •Korea:917-921MHz

                            Note:AlwayscomplywithlocalRFregulationsbeforemodifyingthis

                            setting.

              [4]TagFocus   •EnablestheRFIDreadertoimproveaccuracybyfocusingonasingle
              (Onlysupportedby tagandreducinginterferencefromsurroundingtags.

              E-serieschips) •suitablefordensetagenvironment.

              [5]InventoryBank Defineswhichmemorybankanddatasectionarereadduringtag

                            inventory:

                            •EPC:readstheelectronicproductcodeonly.

                            •EPC+TID/EPC+USER/EPC+RESERVED:readsadditionaltagdata
                            areas.

                            •FastTID:quicklyretrievestheTID(TagID)forfasteridentification.

                            •EPC+EPC:readsduplicateEPCsegmentsforverificationusecases.

                            Note:“Address”and“Length”parametersspecifythestartpositionand

                            wordlengthofthedatatoread.

                                        21
```

### Page 27

```text
4.6 Filter

               ThisscreenallowsuserstofilterorexcludeRFIDtagsduringinventorybasedonspecificdata

            patterns.Ithelpsfocusonparticulartagsorremoveunwantedtagdataforcleanerresults.

              FilterInformation SpecificOption    Description

                FilterMode NormalMode Suitableformostscenarios.
              (determinesthe
                          Professional Enablesadvancedfilteringwithmanualcontrolof
              filtercomplexity
                          Mode       memorybank, addressandmaskdata.
              level)

                FilterBank EPC       FiltersbasedonElectronicProductCode(default).

              (specifieswhich
                          TID        FiltersusingtheTagIdentifierarea(uniquetoeachtag).
              memoryareaofthe
              tagtoapplythe USER     Filtersbasedonuser-definedmemorycontent.

                                        22
```

### Page 28

```text
FilterInformation SpecificOption    Description

              filter)

              StartingAddress StartingAddress Thebitpositionwithintheselectedmemorybankwhere

               &FilterData           filteringbegins.

                          FilterData Thehexadecimalvalueusedasthefiltercondition.

                                     e.g.,Entering3008willmatchtagscontainingthis
                                     pattern.

               FilterSettings PartialExclude Excludestagswherepartofthedatamatchesthefilter.

              (defineshowtags        e.g.,Input“123”filtersouttags123455,645674123but

              areprocessedwhen       keeps14552443.

              theirdatamatches
                          ExactExclude Excludestagsthatexactlymatchthefiltervalue.
              thefiltercriteria)
                                     e.g.,Input“123456”filtersouttag123456butkeeps
                                     123456789,33123456.

                          PartialInclude Displaysonlytagswithdatapartiallymatchingthe

                                     input.

                          ExactInclude Displaysonlytagswhosedataexactlymatchtheinput.

                          NONE       Displaysalltagswithoutfiltering.

              Note:Aftersettingallaboveparameters,pleaseclicktheSAVEbuttontoapplyandactivatethe

              currentfilterconfiguration.

                                        23
```

### Page 29

```text
4.7 Data Output

               Thisscreenprovidestoexportdetectedtag

            inventoryresults,whichbenefitsuserstobackupor

            analyzedataexternally.

            Themainoption“ExporttoExcel”generatesaform
            containingallthenon-repetitivescannedtagdata.

            Exportedfilesarestoredinthepathshownonthe

              page.UserscanlateropenthefileonaPCor

              mobiledeviceforfurtheranalyze.

            4.8Inventory LEDScreen Description

                                              Thisscreenisdesignedfordemonstrating

                                           thefunctionofRFIDLEDtag.Itallowsusersto

                                           performLEDtaginventoryandtriggerLED
                                           lightactivationoncompatibleRFIDtags

                                           throughRFcommunication.

                                           1. Purposeofthisfunction

                                              Thisscreenisprimarilyusedfor

                                           engineeringtesting,fielddemonstrations,or

                                           verifyingtagresponsiveness.TheInventory
                                           LEDfeatureismainlyusedtoverifyand

                                           showcasetheLEDlightcontrolfunctionof

                                           certainRFIDtags.Currently,thisfunctionis

                                           limitedtoonlytwospecificLEDtag

                                           manufacturersnamedKLWandYLthat
                                           supportRF-triggeredLEDactivation.However,

                                           otherstandardRFIDtagsmaynotrespondto

            LEDactivationcommands.

                                        24
```

### Page 30

```text
2. Suggestionsforusing

            •ChoosethecorrectmanufacturerbeforestartinginventorytoensureLEDcommandcompatibility.

            •Whenscanning,compatibletagswillhavetheirLEDindicatorblinkuponactivation.

            Note:Pleasecontactyoursalesrepresentativeortechnicalsupportpersonneltoobtaincompatible

            LED-enabledtags.AsforothernewLEDtag
            brands,pleasecoordinatewithUrovotechnical

            supporttoensureLEDindication

            compatibility.

            4.9 RFID Sled

               Thisscreenprovidesanoverviewofthe

            RFG91RFIDHandle’soperationalstatusand

            allowsuserstoconfiguretimeoutandbuzzer

            parameters.Itservesasadiagnosticand
            controlpanelforcheckingserialnumber,

            firmwareversion,BLEprotocolversionand

            automaticbehaviorsettings.

              DeviceInformation Interpret         Description

              Basicinformation Provideskey DeviceSN:displaysthesled’suniqueserialnumber.

                          identification
                                     FirmwareVersion:showsthecurrentfirmwareversion
                          andfirmware
                                     installedontheRFIDsled.
                          detailsforthe
                          connectedsled. BLEProtocolVersion:indicatesthecurrentBluetooth

                                     LowEnergy(BLE)protocolversionusedfor

                                     communicationwiththehostdevice.

              Buzzerlevel Adjuststhe Thevolumeofferstensettings,incrementingfromthe

                          volumeofRFID lowest(1)tothehighest(10).

                                        25
```

### Page 31

```text
DeviceInformation Interpret         Description

                          reading

              TimeoutSettings Controlsthe ShutdownTimeout(s):setsapre-configureddelay

                          power-saving periodfrom10secondsto6minutesbetweenwhena

                          behaviourofthe shutdowncommandisissuedandwhenthesledis

                          RFIDsled   poweredoff.
                                     e.g.150secondsmeansthesledshutsdownifactivefor

                                     150seconds.

                                     SleepTimeout(s):setsaperiodofuserinactivityfrom

                                     10secondsto6minutesafterwhichthesled

                                     automaticallyentersalow-powersleepmode.
                                     e.g.110secondsmeansthesledsleepsafter110

                                     seconds110secondsofinactivity.

            5.  Optional Accessory

               Comparedtoastandardcharger,adedicatedcradlechargerdeliversasuperioruserexperience.Its

            keyadvantagesincludetheabilitytochargetwodevicesatonce,keepthemorganizedinanaccessible

            position,andfeaturesmartindicatorssuchasthedynamicalbattery-levelscreensaveroftwodevices

            DT610andRFG91handleforat-a-glancestatusupdatesduringcharging.Oncetwodevicesare
            removedfromthecradlecharger,thescreenautomaticallyrevertstothesystemdefaultscreensaver.

                                        26
```

### Page 32

```text
6. FAQ

            6.1 Connection Issues

            Q1:IftheRFIDdemocan’tdetecttheRFG91,whatshouldIdo?

            A:Pleaseensurethefollowing:
            1. TheRFG91powerswitchisturnedonbeforeopeningtheRFIDdemoapplication.

            2. ForthePogoversionoftheRFG91RFIDhandle,thedeviceisfirmlyattachedtothe

            handle.Ifnot,pleasereconnectthedevicefirmlyuntilyouhearaclickorfeelsecurecontact.

            3. Thereaderconnectionwiththedeviceiscorrect.

            • ForPogoversion:chooseWiredConnection.

            • ForBluetoothversion,chooseWirelessConnectionandthenpairviaQRcode,NFCtap,or

            manualsearch.

            Q2:WhydoestheBluetoothversionofRFG91pairunsuccessfully?

            A:Possiblecausesandsolutions:

                                        27
```

### Page 33

```text
1. Thehandlehasanactiveconnectionwithanotherdevice.

            Solution:LongpresstheBluetoothbuttonontheRFG91toforce-disconnectandretry

            pairing.

            2. DevicenotinpairingmodeorBluetoothdisabledonthehandheld.

            Solution:EnableBluetoothandrestartboththehandleandtheapplication.
            3. TheRFIDdemohascrashed.

            Solution:Forgetthedevicefromthesystempairedlist,andusetheapplicationtopairagain.

            6.2 Reading / Tag Detection Issues
            Q3:Whyistherenotagdetected?

            A:Possiblecausesandsolutions:

            1. Thereaderantennaiscoveredorfacingawayfromtags.

            Solution:Adjustthereaderdirectionanddistancefromtherangeof0.5metersto2meters.

            2. TagfrequencymismatchesRFspectrumofthehandle.

            Solution:VerifytheregulatoryregioninSettings.

            3. RFoutputpowerissettoolow.

            Solution:IncreasethepowerleverunderRFoutputpowerofbasicsettings,andthensaveand
            testagain.

            Q4:Ifonlyafewtagsaredetectedorscanningisunstable,whatshouldIdo?

            A:

            1. Itissuggestedtotestinanopenenvironmentawayfrommetalordenseliquidcontainers,

            becauseofEnvironmentalinterferenceortoomanyreflectivesurfaces.

            2. Youcanincreasetherefreshrateintheappsettingstoimproveuserperceptionanddata
            updatespeed.

            Q5:Whydothetagsfailedtobereadorwritteneveniftheyweredetected?

            A:

                                        28
```

### Page 34

```text
1. Cause:tagmemorybankoraddressisconfiguredincorrectly.

            Solution:VerifythatEPC/TID/USERmemorybankiscorrectlyselectedbefore

            performingread/writeoperations.

            2. Cause:tagaccesspasswordisinsufficientorlocked.

            Solution:ChecktagaccesspermissionorperformUnlockbeforewritingorkillingthetag.

            6.3Application Function Issues

            Q6:Thereisnoconfirmationfeedbackafterclicking“SAVE”,what’sthenextstep?

            A:Pleaseensuretheappdisplaysatoastmessagesuchas“Settingssavedsuccessfully”.
            Ifnot,reconnectthehandleandtryagain.

            Q7:WhatcanIdowhendataexportisfailedorthefileismissing?

            A:Pleaseperformatagscanfirst,becauseexportfunctionisdisabledwhenthereisnodata

            exist.

            Ensurethedevicehasfilewrittenpermission.Ifnot,pleasegranttheappstoragepermission

            andretryexporting.

            6.4 Performance and Displays Issues

            Q8:Howcanthetagcountrefreshquickly?

            A:Optimizerefreshrateorenablehigh-performancemodesuchasRapidRepeatmodeunder
            PerformanceMode.

            Q9:What’sthenextstepoccurringtoapplicationcrashduringthecontinuous

            inventory?

            A:Thismaybecausedbytoomanytagsorlongscanningduration.

            Recommendedactions:

            1. Stopscanningperiodically.
            2. limitmaximumtagcountdisplay.

                                        29
```

### Page 35

```text
3. Restarttheappifperformancedrops.

            6.5 Hardware Issues

            Q10:Thehandlebeepscontinuously.Whatisthereason?

            A:Thisisprobablylowbatteryorerrorwarning.YoucouldrechargetheRFG91handleand

            ensurethepowerisstable.

            Q11:HowcanIevokethehandleinsleeporshutdownmode?

            A:PressthepowerButtonfor3secondstowakeitup,orreinsertthedevicetoreinitializethe
            connection.

            7 . Error Code and Troubleshooting Guide

               ThissectionprovidesdetaileddescriptionsofcommonRFIDDemoerrorcodesand
            troubleshootingstepsforresolvingtypicalissuesencounteredduringtestingordeployment.

            7.1 Error Code Table

               ErrorCode  ErrorMessage    Description   Troubleshooting

             TAG_NOT_FOUN NoRFIDtag   Thereaderdidnotdetectany Movethetagcloser,adjust

             D           detectedinfield tagwithinitsfield. antennaorientation,increase

                                                      RFpower.

             INSUFFICIENT_PO Tagpower Thetagisnotreceiving Reducedistance,increaseRF
             WER         insufficientfor enoughenergytocompletea outputpowerinSettings→

                         memorywrite  write.          RFID,avoidinterference.

                         operation

             MEMORY_ERROR Memory      Requestedmemoryaddress Verifymemorybank/address

                         out-of-boundsor isinvalidorPCfieldis andconfirmtagsupportsthe

                         unsupportedPC unsupported.   requestedarea.
                         value

                                        30
```

### Page 36

```text
ErrorCode  ErrorMessage    Description   Troubleshooting

             MEMORY_LOCKE Memorybank  Targetmemoryregionis Useread-onlyoperationsor

             D           permanentlylocked, permanentlylockedand replacethetagifmodification

                         writeprohibited cannotbewritten. isrequired.

             ACCESS_PWD_ER Accesspassword Providedaccesspassword Re-enterthecorrectaccess

             ROR         incorrect    doesnotmatchthetag. password,verifywithtag

                                                      configuration.

             TAG_UNKNOW_E Thelabelhasan Tagrespondedwithan Retrytheoperation,
             RROR        unknownerror,and unknown/uncategorized power-cyclethereader,test

                         theerrorcodewas error.       withaknown-goodtag.

                         notcaptured

             KILL_PWD_ERRO Killpassword Killpasswordverification Checkandre-enterthecorrect

             R           incorrect    failed.         killpassword.

             INVALID_KILL_P Killpasswordcannot All-zerokillpasswordis Useavalidnon-zerokill

             WD          beallzeros   invalidperEPCGen2spec. password.

             UNSUPPORTED_C Tagdoesnotsupport TheattemptedEPC/ISO Consultthetagdatasheet;
             MD          thiscommand  commandisnotsupportedby avoidunsupported

                                      thistagtype.    commands.

             INVALID_ACCESS Accesspassword Thecommandrequires Providetheaccesspassword

             _PWD        requiredforthis authenticationwithanaccess beforeexecutingthe

                         command      password.       command.

             READ_PROTECTE Tagalready Thetag’smemoryis Removeprotection(if

             D           read-protected protectedagainstreads. possible)orproceedwith
                                                      permittedoperationsonly.

             NOT_READ_PROT Tagnot     Unlock/read-protect Continuewithoutunlock;no

             ECTED       read-protected, operationisunnecessary. actionneeded.

                         unlocknotrequired

             GENERIC_ERROR Non-specifictag Agenericfailureoccurredon Retryandensure

                                        31
```

### Page 37

```text
ErrorCode  ErrorMessage    Description   Troubleshooting

                         error(nodetailed thetagside. firmware/appversionsareup

                         code)                        todate.

             WRITE_FAILED Writefaileddueto Writeattemptfailedbecause Unlockthememoryregion(if

                         lockedmemory theblocksarelocked. supported)orchooseanother

                         blocks                       writablearea.

             LOCK_FAILED Memorylock   Theattempttosetlockbits Retryafterresettingthe
                         operationfailed didnotsucceed. session;verifyparameter

                                                      values.

             ALREADY_LOCK Memoryalready Thetargetmemoryisalready Cannotmodify;usea

             ED          permanentlylocked permanentlylocked. differentmemoryareaor

                                                      replacethetag.

             PARAM_SAVE_FA Parametersavefailed Parameterswerenot Retrysaving;ensurestable

             ILED        (volatileuntilreader persistedtonon-volatile powerandconnectiontothe
                         power-off)   storage.        reader.

             ADJUST_FAILED Parameter  Arequestedparameter Validateparameterrangeand

                         adjustmentfailed changecouldnotbeapplied. reattempt.

             ANTENNA_ERRO Antennadetection Readerfailedto Checkhardware

             R           failure      detect/initializetheantenna. connection/pogopins;reseat

                                                      andretry.

             CMD_EXEC_FAIL Commandexecution Readerreturnedafailure Retry;verifycommand

             ED          error        whenexecutingthe syntaxandparameters.
                                      command.

             COMMUNICATIO Tagdetectedbut Thesignalisweakor Reduceinterference,shorten

             N_FAILURE   communication unstablecausingintermittent distance,andreorient

                         unstable     communication.  antenna.

             NO_TAG      NooperableRFID Notagiscurrently Ensurethetagispresentand

                         taginfield   operable/respondinginthe compatible;movecloser.

                                        32
```

### Page 38

```text
ErrorCode  ErrorMessage    Description   Troubleshooting

                                      field.

             TAG_ERROR   Tagreturnederror Thetagexplicitlyreturnedan Testwithanothertagto

                         code         errorstatus.    isolatetag-specificfaults.

             INVALID_CMD_L Invalidcommand Suppliedcommandframe CheckSDKpacket

             ENGTH       length       lengthisinvalid. formattingandparameter

                                                      sizes.

             ILLEGAL_CMD Illegalcommandfor Commandisnotallowedin Reinitializeinventory/session
                         currenttagstate thetag’scurrent andreattempt.

                                      state/session.

             PARAM_ERROR Invalidcommand Oneormoreparametersare Correctparametervaluesand

                         parameters   invalidoroutofrange. retry.

             INVALID_INVENT Inventorymodenot Selectedcustominventory Resettoasupportedmode

             ORY_MODE    incustom     modeisinvalid.  underPerformanceMode.

                         configuration

             UNSUPPORTED_F Firmwaredoesnot Thecurrentfirmwarelacks Upgradereaderfirmwareto
             EATURE      supportthisfeature thiscapability. thelatestversion.

             COMMUNICATIO RFcommunication GeneralRF   Reconnectthereaderand

             N_ERROR     error        transmission/handshake restarttheapp.

                                      failure.

             SDK_UNINITIALI SDKnotinitialized SDKAPIswerecalled Callinit()atstartup;restart

             ZED                      beforesuccessful theappifneeded.

                                      initialization.

             DEVICE_DISCON RFIDreadernot Theexternal/BTreaderis Reconnect
             NECTED      connected    disconnected.   Bluetooth/pogo/USBand

                         (external/BTdevice)          reopentheapp.

             SEND_CMD_FAIL Command    Theappfailedtosendthe CheckBLEsignal/cable,

                         transmissionfailed           reconnectthehandle,and

                                        33
```

### Page 39

```text
ErrorCode  ErrorMessage    Description   Troubleshooting

             ED          (external/BTdevice) commandtothedevice. retry.

            7.2 Troubleshooting Procedure

               FollowthesestepssystematicallywhenencounteringissueswiththeRFIDDemoapplicationor

            RFG91RFIDreader.

                     Step                      Description

            CheckConnection      ConfirmtheRFG91handleispoweredonandpaired
                                 (BluetoothorPogo).

            VerifyPowerLevel     Ensuresufficientbatterypowerandtagdistancewithin50cm.

            Reboot&Retry         RestartbothDT610andRFG91handletoclearsessioncache.

            TestwithKnownGoodTag Useaverifiedtagtoruleouttag-specificdefects.

            UpdateFirmware       UpgradetothelatestOSandRFG91firmwareversions.

            CheckSDKInitialization Ensureinit()iscalledbeforeinvokingtagoperations.

            EnableLogs           Collectlogsfrom/sdcard/RFIDDemo/foranalysis.

            ContactUrovoSupport  Providelogsandfirmwareversiontotechnicalsupportfor

                                 furtherassistance.

            8. Care and Maintenance

              TherearesomesuggestionsfordailyusingtheRFG91handle:
            1. AlwaysensurebothfirmwareandRFIDDemoappareupdatedtothelatestversions.

            2. Whenswitchingdevicesormodules,performafullreconnectioninsteadofhot-swapping.

            3. Foroptimallong-termbatteryhealth,itisrecommendedtominimizeusingthehandle

            duringcharging.

            4. Ifissuesstillexist,capturealogcattraceandcontactUrovotechnicalsupportforanalysis.

                                        34
```
