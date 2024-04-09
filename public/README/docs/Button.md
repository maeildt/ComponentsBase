[`◀️Homepage`](../../../README.md)

# **Button** 


**import**
>           import M_Button from 'src/components/M_Components/M_Button/M_Button'
  


## **Basic**

To create a basic button like this, you only need to use the 'label' and 'onClick' properties.


<div style="display:flex;justify-content:center;margin:10px;background:#EBEDED;border-radius:5px">

![Alt text](../../../public/README/images/button.png)
    
</div>

>            <M_Button label={'Button'} onClick={() => do something()} />



## **Colors**

You can customize your buttonby changing the color of your border, background and label color using borderColor, backgroundColor, labelColor and defining what color you want:

<div style="display:flex;justify-content:center;margin:10px;background:#EBEDED;border-radius:5px">

![Alt text](../../../public/README/images/buttonBorder.png)
![Alt text](../../../public/README/images/buttonBackground.png)

</div>

>            <M_Button borderColor={'pink'} label={'Button'} onClick={() => do something()} />
> 
>            <M_Button backgroundColor={'pink'} label={'Button'} onClick={() => do something()} />



## **Icons**

Adding icons to your button is strictly done with html elements to increase customizability. You can add them with the icon property and set its location with iconPosition (right or left)

<div style="display:flex;justify-content:center;margin:10px;background:#EBEDED;border-radius:5px">

![Alt text](../../../public/README/images/buttonOnlyIcon.png)
![Alt text](../../../public/README/images/buttonIcon.png)
    
</div>

 >          <M_Button icon={<img src='/icons/svgsDaNet/user.svg' />} borderColor={'black'} onClick={() => do something()} />
 >
 >          <M_Button iconPosition={'left'} icon={<img src='/icons/svgsDaNet/user.svg' />} borderColor={'black'} label={'Button'} onClick={() => do something()} />

## **Size**

Changing size is done by simply adding the word *small*, *normal* or *large* to the M_Component

<div style="display:flex;justify-content:center;margin:10px;background:#EBEDED;border-radius:5px">

![Alt text](../../../public/README/images/buttonSmall.png)
![Alt text](../../../public/README/images/buttonNormal.png)
![Alt text](../../../public/README/images/buttonLarge.png)
 
</div>


>           <M_Button small borderColor={'black'} label={'Button'} onClick={() => do something()} />
>
>           <M_Button normal borderColor={'black'} label={'Button'} onClick={() => do something()} />
>
>           <M_Button large borderColor={'black'} label={'Button'} onClick={() => do something()} />


# **Drawer**

You can use any combination of settings to open a drawer as long as you defined the properties *element* if you want a personalized drawer ( you pass the html elements), *entity* if you weeant a table drawer ( here you defined what table to use), *tableLabel* when using a tableDrawer to define the drawer name, *getLine*, function that returns the line you select on the table, *FILTER* filter string used to filter the table 

![Alt text](../../../public/README/images/buttonDrawer2.png)

>                       <M_Button element={<span> THIS IS AN ELEMENT DRAWER</span>} label={'teste'} icon={<img style={{ filter: ' invert(100%) sepia(0%) saturate(4800%) hue-rotate(288deg) brightness(104%) contrast(94%)' }} src='/icons/svgsDaNet/user.svg' />} backgroundColor={'var(--color-blue-light)'} labelColor={'white'}  />





## **Other features**

| Properties           	| Description                                          	| Example                                        	|
|----------------------	|------------------------------------------------------	|------------------------------------------------	|
| onClick              	| Passed function is executed on click                 	| onClick={()=>function()}                       	|
| borderColor          	| color the border                                     	| borderColor={'black'}                          	|
| backgroundColor      	| color the background                                 	| backgroundColor={'black'}                      	|
| label                	| Button Label                                         	| label={'Button'}                               	|
| labelColor           	| color the button label                               	| labelColor={'white'}                           	|
| icon                 	| icon element                                         	| icon={<img src='/icons/svgsDaNet/user.svg' />} 	|
| iconPosition         	| position of the icon ( left or right)                	| iconPosition={'right'}                         	|
| tooltip              	| tooltip string                                       	| tooltip={'Button'}                             	|
| small, normal, large 	| used to set button size                              	| small, normal, large                           	|
| element              	| html elements to pass inside a drawer                	| element={<span>example</span>}                 	|
| entity               	| entity name to use for the table drawer              	| entity={'account}                              	|
| tableLabel           	| label used inside the table drawer                   	| tableLabel={'LABEL'}                           	|
| getLine              	| function that returns the line selected on the table 	| getLine={() => {}}                             	|
| FILTER               	| string used to filter the table in the drawer        	| '(Field Name) (eq /contains) (value)'          	|
| disable              	|                                                      	| true or false.                                 	|