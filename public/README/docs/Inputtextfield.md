[`◀️Homepage`](../../../README.md)

# **Input TextField** 


**import**
- *`import M_InputTextField from 'src/components/M_Components/M_InputTextField/M_InputTextField'`*

**Basic**

To create a text field like this, you only need to use the label, onChange and color properties.

![Alt text](../../../public/README/images/inputTextField.png)

>         <M_InputTextField label={"Client Reference"} onChange={(e) => e.target.value} color={'var(--color-blue)'} />

**Other features** 

| Properties  | Description                                 | Example                                                                |
| ----------- | ------------------------------------------- | ---------------------------------------------------------------------- |
| type        | Pass a type to active type                  | date, datetime-local, email, number, text, password, search, tel, time |
| value       | Pass a value or ""                          | value={value}                                                          |
| disabled    | If true, the component is disabled          | disabled={false}                                                       |
| required    | true or false                               | required={true}                                                        |
| secondColor | Pass a color to use this property           | secondColor={'var(--color-blue)'}                                      |
| letterColor | Pass a color to use this property           | secondColor={'var(--color-blue)'}                                      |
| size        | Pass a size to use this property            | auto, medium or small                                                  |
| iconStart   | Insert button at the start of the textfield | iconStart={<Clear />}                                                  |
| iconEnd     | Insert button at the start of the textfield | iconEnd={<Clear />}                                                    |