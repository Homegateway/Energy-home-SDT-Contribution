# Mapping the Energy@home data model to SDT 3

The [Energy@home data model](http://www.energy-home.it/Documents/Technical%20Specifications/E@h_data_model_v2.1.pdf) is an extension of [IEEE 2030.5](http://standards.ieee.org/findstds/standard/2030.5-2013.html), therefore the SDT 3 mapping defined in this repository is also valid for that standard. The foundamental characteristic of this data model is its adherence to RESTful design principles, which implies that all operations are mapped to standard HTTP methods (i.e. GET, POST etc.). The SDT 3 mapping is constructed as follows: 

- Top-level resources are mapped to modules, and the module's data contain the resource's representation; top-level resources may also contain sub-resources. 
- The hyperlinks between different resources are represented via the 'uri' data type. 
- The HTTP POST method is represented by an action associated to the module whose name begins with 'Create' 
- The HTTP DELETE method is represented by an action associated to the module whose name begins with 'Delete'. 
- The GET and PUT methods are not explicitly described by actions, as they are simply associated to the reading or writing of data points. 
- The HTTP HEAD method is not described. 
- The resources which can generate events will also have SDT events associated to the corresponding module. 


