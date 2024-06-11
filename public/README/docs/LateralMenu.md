[`◀️Homepage`](../../../README.md)

# **Lateral Menu** 


**import**
- *`import M_LateralMenu from 'src/M_Components/M_LateralMenu/M_LateralMenu'`*

**Basic**

To create a basic lateral menu like this, you only need to use the showMenu, menus, setMenus and bodyPage properties.

![Alt text](../../../public/README/images/LateralMenu.png)
>
>       const tempMenu = [
>           {
>               "menuLabel": "LabelCurrentSeason",
>               "menuIcon": <Album />,
>               "menuOpen": false,
>               "subMenus": [
>                   {
>                       "subMenuLabel": "LabelPractitioners",
>                       "subMenuDisplay": "LabelPractitioners",
>                       "subMenuOpen": false,
>                       "subSubMenus": [],
>                       "tableName": "Practitioner",
>                       "subMenuUrl": "season/practitioners"
>                   },
>                   {
>                       "subMenuLabel": "LabelTeams",
>                       "subMenuDisplay": "LabelTeams",
>                       "subMenuOpen": false,
>                       "subSubMenus": [],
>                       "tableName": "Team",
>                       "subMenuUrl": "season/teams"
>                   },
>               ]
>           },
>           {
>               "menuLabel": "LabelActions",
>               "menuIcon": <Album />,
>               "menuIconFilter": "invert(41%) sepia(74%) saturate(4623%) hue-rotate(354deg) brightness(91%) contrast(104%)",
>               "menuOpen": false,
>               "subMenus": [
>                   {
>                       "subMenuLabel": "LabelResultsAndOccurrences",
>                       "subMenuDisplay": "LabelResultsAndOccurrences",
>                       "subMenuOpen": false,
>                       "subSubMenus": [],
>                       "tableName": "Occurrence",
>                       "subMenuUrl": "actions/resultsAndOccurrences"
>                   },
>                   {
>                       "subMenuLabel": "LabelSectionAnalysis",
>                       "subMenuDisplay": "LabelSectionAnalysis",
>                       "subMenuOpen": false,
>                       "subSubMenus": [],
>                       "tableName": "SectionAnalysis",
>                       "subMenuUrl": "actions/sectionAnalysis"
>                   },
>               ]
>           },
>        ]
> 
>       const [menus, setMenus] = useState(tempMenu)
> 
>       <M_LateralMenu showMenu={showMenu} menus={menus} setMenus={setMenus}  />

**Other features**

| Properties 	| Description                                                                                         	| Example                                                                                                                                                                                                                                         	|
|------------	|-----------------------------------------------------------------------------------------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| showMenu   	| boolean. Opens and closes the menu                                                                  	| showMenu={true}                                                                                                                                                                                                                                 	|
| menus      	| array of object used to build the menu. Pass in State value                                         	| menus={[{menuLabel:"button1",menuIcon:Icon,menuImg:"src",menuStyle:{color:'red'},menuOpen:false,subMenu:[{subMenuLabel:"subButton",subMenuDisplay:"Button",subMenuOpen:false,subSubMenus:[],tableName:"Table",subMenuUrl:"master/country""}]}]} 	|
| setMenus   	| pass in set value state                                                                             	| setMenus{setMenus}                                                                                                                                                                                                                              	|
| bodyPage   	| The rest of the page next to the tabs                                                               	| div input div                                                                                                                                                                                                                                   	|
| lngMenu    	| language option buttons. Array of objects.                                                          	| [{menuLabel:"PT",menuImg:"src",menuIcon:"Icon",onClick:() = changeLng()}]                                                                                                                                                                       	|
| lastMenus  	| Array of object. Last buttons that show on the bottom. Usually used for settings and logout buttons 	| [{menuLabel:"settings",onClick:() = setShowMenu(false),menuIcon: icon}]                                                                                                                                                                         	|
| footerName 	| label on the bottom of the menu. Used to show the name of the user / company. string                	| footerName={"Duarte \| Devlop"}                                                                                                                                                                                                                 	|                               |

