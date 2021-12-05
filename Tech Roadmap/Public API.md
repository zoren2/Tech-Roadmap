# Public API

A javascript framework or back-end language can consume a public facing API then programmatically serve the results to the user.

Javascript fetch() allows you to consume a public facing API if given a particular key. Then you can dereference those objects in order to process whatever you want from the API fields.

If you use an intermediate back-end language such as [[C#]], you're likely to use some kind of ORM in order to create object models which you can then dereference and operate on using the [[dot NET Runtime]] operations and libraries inside user defined custom classes.

These models then get passed to a view which is then operated on by [[Razor]] views which allows you to embed specific language logic inside [[HTML]].