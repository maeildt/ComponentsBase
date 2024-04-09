[`◀️Homepage`](../../../README.md)

# **Router** 


**import**
- *`import M_Router from 'src/components/M_Components/M_Router/M_Router'`*

**Basic**


>            <M_Router
>               primaryColor={"var(--color-blue)"}
>               secondaryColor={"var(--color-blue-dark)"}
>               endpoints={['booking']}
>               url={DefaultURl}
>               Routing={
>                 <Router>
>                   <Routes>
>                     <Route path="*" element={<Page404 />} />
>                     <Route path="/home/*" element={<HomePage />} />
>                     <Route path="/login" element={<LoginPage />} />
>                   </Routes>
>                 </Router>}

**Other features**

| Properties | Description                                 | Example                  |
| ---------- | ------------------------------------------- | ------------------------ |
| primaryColor       | primary color to be used in all the project |                          |
| secondaryColor    | secondary color to be used in all the project         | |
| endpoints      |array of endpoints to highjack and replace with a "/query?"         |                |
| url       | url for the backend side           |                          |
| Routing     | used to create routes as seen above             |                          |