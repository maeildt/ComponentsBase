[`◀️Homepage`](../../../README.md)

# **Switch Button** 


**import**
- *`import M_SwitchButton from 'src/components/M_Components/M_SwitchButton/M_SwitchButton'`*

**Basic**

To create an interrutor like this, you just need to use the label and color properties.

![Alt text](../../../public/README/images/SwitchButton.png)
>            <M_SwitchButton color={"var(--color-blue)"} label="Created By"/>

**Other features**

| Properties     | Description                                         | Example                  |
| -------------- | --------------------------------------------------- | ------------------------ |
| checked        | If true, the component is checked                   | checked={false}          |
| onClick        | Pass a function to active onClick                   | onClick={()=>function()} |
| required       | If true, the input element is required              | required={true}          |
| disabled       | If true, the component is disabled                  | disabled={false}         |
| defaultChecked | The default checked state                           | defaultChecked={false}   |
| tooltipName    | Label to show tooltip                               | tooltipName={"tooltip"}  |