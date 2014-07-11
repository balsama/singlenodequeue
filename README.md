#Single Node Queue

##Purpose
Projects often include a single promoted item, such as a featured Article or
promoted News Story. This is often accomplished by adding a "Promoted" field
to the content type. However, this approach becomes problematic because,
eventually, more than one node will be promoted unless an expensive check for
other promoted content is perfomed on each node save.

This module uses a different approach by selecting the node to be promoted
outside of the node itself. (That is, the node doesn't inherntly "know" that it
is promoted.) **It provides an admin interface to select a single node to be
promoted.**

##Similar Modules
The Node Queue module provides similar (and a lot more) functionality. But it
comes with so many options that it often confuses admins who just want to
promote a single piece of content.

##Roadmap
* Provide admin interface to select the valid content types for promotion.
* Allow a site to have more than one SNQ.
* View integration.
* Helper function that returns the current promoted NID (currently you have to
  use `variable_get()`.

