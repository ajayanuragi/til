# Matrix variables:

## Matrix variables are a block/segment of values that travel along with the URI. For example, /localRate=1,2,3/

These variables may appear in the middle of the path unlike query parameters which appear only towards the end of the URI.

Matrix variables follow name=value format and use semicolon to get delimited from one other matrix variable. 

A matrix variable can carry any number of values, delimited by commas.

@MatrixVariable is used to extract the matrix variables.
---
Example: Assume, there is a REST controller called PlanController that has a service to return the details of Plans based on the search criteria, localRates.

Below is the URI path. Observe that a variable localRate with two values separated by "," appear in the middle of the path.

```
URI:http://<<hostname>>:<<port>>/<<contextpath>>/plans/localRate=1,4 /plan
```
