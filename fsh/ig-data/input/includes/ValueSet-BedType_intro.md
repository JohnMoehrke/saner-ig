The vocabulary for the type characteristic is informed by the work of AHRQ,
ANSI/HITSP, HL7, and OASIS in advancement of the OASIS HAVE standards, and the
AHRQ [HAvBED](https://archive.ahrq.gov/prep/havbed2/) specification.

<table class='grid'>
<thead>
<tr><th>Code(s)</th><th>HAVE Category</th><th>HAVE/HAvBed Description</th></tr>
</thead>
<tbody>
<tr><td>ICU</td><td>AdultICU</td><td>Adult ICU bed type<br/>These can support critically ill or injured patients, including ventilator support
This category includes all major subtypes of ICU beds, including neurological, cardiac, trauma, or medical, with the exception that this category does not include burn ICU beds</td></tr>
<tr><td>PEDICU</td><td>PediatricICU</td><td>Pediatric ICU beds.<br/>This is similar to adult ICU beds, but for patients 17-years-old and younger.</td></tr>
<tr><td>PEDNICU</td><td>NeonatalICU</td><td>Neonatal ICU beds</td></tr>
<tr><td>ER</td><td>ED</td><td>Emergency Department beds used for acute care</td></tr>
<tr><td>NURSERY</td><td>NurseryBeds</td><td>Capacity Status for Neonatal or newborn care beds including all bed types other than Neonatal ICU</td></tr>
<tr><td>HU</td><td>MedicalSurgical</td><td>Medical-surgical beds<br/>
These are also thought of as ward beds.
These beds may or may not include cardiac telemetry capability</td></tr>
<tr><td>RHU</td><td>RehabLongTermCare</td><td>Rehabilitation/Long term care beds<br/>
Beds designated as long term care rehabilitation. These do not include floor beds</td></tr>
<tr><td>BURNU</td><td>Burn</td><td>Burn beds<br/>
These are thought of as burn ICU beds, either approved by the American Burn Association or self-designated.
These beds are NOT to be included in other ICU bed counts.</td></tr>
<tr><td>PEDU</td><td>Pediatrics</td><td>Pediatrics beds. <br/>These are ward medical/surgical beds for patients 17-years-old and younger
<tr><td>PHU<sup><a href='#fn1'>1</a></sup></td><td>Psychiatric</td><td>Ward beds on a closed/locked psychiatric unit or ward beds where a patient will be staffed by an attendant.</td></tr>
<tr><td>NEGISO</td><td>NegativeFlowIsolation</td><td>Negative airflow isolation beds.<br/>These provide respiratory isolation.
NOTE: This value may represent available beds included in the counts of other types</td></tr>
<tr><td>OTHISO</td><td>OtherIsolation</td><td>Isolation beds.<br/>These provide isolation where airflow is not a concern.
NOTE: This value may represent available beds included in the counts of other types</td></tr>
<tr><td>OR<sup><a href='#fn2'>2</a></sup></td>
    <td>OperatingRooms</td>
    <td>Operating rooms which are equipped, staffed and could be made available for patient care in a short period of time</td>
</tr>
</tbody>
</table>

NOTE: NURSURY, BURNU, OR, NEGISO, OTHISO and NONISO come from the [SANER Bed Type Code
System](CodeSystem-SanerBedType.html) which was created to fill the gaps in existing
FHIR R4 Coding Systems.

