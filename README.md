# MUON
µON is object notation format with some good properties for M2M communication.
µ[mju:] stands for "micro", like microcontroller is sometimes abbreviated "µC".

µON primitive types:
* String
* Blob (binary)

µON composite types:
* List (sequence of elements)
* Dict (associative container of key-value pairs)
* Meta (a Dict that contains meta-information )

µON features:
* Easily parseable, even on microcontrollers
  * Actually you can just interpret it on-fly
* Supports binary values
* Supports UTF-8 string values
* Unlimited size of objects
* Data can be used "in-place"
* Any JSON or XML document should be convertable to MUON without information/structure loss

µON compared to JSON and XML:
* µON is binary format (so not human-readable)
  * But can easily be transformed into a readable form
* Almost all data is stored in strings.
  * But keys and values are not quoted. They are zero-terminated instead.
  * So there's no need to escape "'&<>...
* "Meta" type is similar to attributes in XML
  * But it is equivalent to Dict, so can contain tree structures
* 
