A Group resource conforming to the Bed Group profile can be computed by counting Location
resources matching the characteristics found in the Bed Group Profile.  The Bed Location
profile describes the essential fields in a Location resource that can be counted in
this way (with the exception of Property, see below).

A Bed is both a medical device that is associated with a specific location (e.g., a
room that it is placed in), and also a location where patient care can be provided.

Most of the attributes about a bed needed by public health can be determined by
fields in the Location resource.

Each characteristic in the Bed Group can be tied back to a FHIR element associated
with the Location resource.

* `Group.characteristic.code` identifies the specific field that is used to obtain the
value for the characteristic.
* `Group.characteristic.valueCodeableConcept` is the matching value for the element
when the field is a coded value.
* `Group.characteristic.valueReference` is the matching value for the element when
the field is a resource reference.

### Property
One location characteristic needs to be called out because it requires special handling,
and that is Isolation.  Isolation is typically a structural feature of the room or
other enclosure that the bed is placed in, rather than a functional feature.  The distinction
is subtle: structure = what it is, functional = how it is used.  A hospital ward room
becomes a labor and delivery room because it is used to deliver a baby (although that
is not its usual function).  An operating room can be repurposed to become an ICU.
But negative airflow isolation is a structural feature (in most cases).  So, while it
might be appropriate in Location to describe this in Location.type, it's not clear if
its appropriate to keep this structural capacity together with the functional capabilities.

So, in this guide, we separate them (it's not clear that it is important to do this,
as one can have multiple characteristics of the same type and support query on them).
From the public health viewpoint, keeping the ability to separate isolation features
from other service delivery features seems important when managing an airborne
illness.