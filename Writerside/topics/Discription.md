# Discription

The RFC Executor Step is the most flexible out of the three steps to communicate with SAP systems. This Step uses the RFC function call to read data from the current database. You are able to do every available RFC function call or BAPI.

Parameters could be import, table or export parameters. Within the field value in the fields table you are able to change the values of the parameter fields, e.g. the name of the query table in RFC_READ_TABLE. The results be converted into JSON and pass to Stream as a String. Otherwise, you get the parameter as key/value pairs. The step supports Metadata Injection.

