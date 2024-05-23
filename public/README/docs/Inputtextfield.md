[`◀️Homepage`](../../../README.md)

# **Input TextField** 


**import**
- *`import M_InputTextField from 'src/components/M_Components/M_InputTextField/M_InputTextField'`*

**Basic**

To create a text field like this, you only need to use the label, onChange and color properties.

![Alt text](../../../public/README/images/inputTextField.png)

>         <M_InputTextField label={"Client Reference"} onChange={(e) => e.target.value} color={'var(--color-blue)'} />

**Other features** 

| Properties            	| Description                                                                                           	| Example                                                                	|
|-----------------------	|-------------------------------------------------------------------------------------------------------	|------------------------------------------------------------------------	|
| label                 	| String. Label for the input.                                                                          	| label={"this is a label"}                                              	|
| maxNumbers            	| Number. Max number Size                                                                               	| maxNumber={3}                                                          	|
| type                  	| Pass a type to active type                                                                            	| date, datetime-local, email, number, text, password, search, tel, time 	|
| value                 	| Pass a value or ""                                                                                    	| value={value}                                                          	|
| disabled              	| If true, the component is disabled                                                                    	| disabled={false}                                                       	|
| required              	| true or false                                                                                         	| required={true}                                                        	|
| placeholder           	| beginning value showed in the input                                                                   	| placeholder={'Search'}                                                 	|
| secondColor           	| Pass a color to use this property                                                                     	| secondColor={'var(--color-blue)'}                                      	|
| onKeyDown             	| Function. Fired on every key pressed                                                                  	| onKeyDown={(e) = doSomething(e.keyCode)}                               	|
| color                 	| Pass a color to use this property                                                                     	| color={'var(--color-blue)'}                                            	|
| size                  	| Pass a size to use this property                                                                      	| auto, medium or small                                                  	|
| iconStart             	| Insert button at the start of the textfield                                                           	| iconStart={}                                                           	|
| iconEnd               	| Insert button at the start of the textfield                                                           	| iconEnd={}                                                             	|
| height                	| height of the input                                                                                   	| height={20}                                                            	|
| padding               	| padding of the input                                                                                  	| padding={20}                                                           	|
| margin                	| margin of the input                                                                                   	| margin={20}                                                            	|
| backgroundColor       	| color of the input background                                                                         	| backgroundColor={20}                                                   	|
| autoFocus             	| auto focuses this input                                                                               	| autofocus                                                              	|
| onEnter               	| function fired when pressing Enter. Best for submit functions                                         	| onEnter={() = submit()}                                                	|
| helperTextMessage     	| string.                                                                                               	|                                                                        	|
| errorMessage          	| string.                                                                                               	|                                                                        	|
| passVerification      	| boolean. if on shows password requirements                                                            	|                                                                        	|
| minLengthverification 	| min number length                                                                                     	| minLengthverification={10}                                             	|
| valueAgain            	|  value used when type is password.  value used to compare if the new Password equals the new Password 	|                                                                        	|
| noAutoShrink          	| boolean. lets the label sit in the center of the input                                                	|                                                                        	|
