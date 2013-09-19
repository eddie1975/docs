{{Page_Title}}
{{Flags
|High-level issues=Needs Review
|Checked_Out=No
}}
{{Standardization_Status|W3C Working Draft}}
{{API_Name}}
{{Summary_Section|A grid item's placement in a grid area consists of a grid position and a grid span. The grid-row-start property (with [[css/properties/grid-column-start|grid-column-start]], [[css/properties/grid-row-end|grid-row-end]], and [[css/properties/grid-column-end|grid-column-end]]) determines a grid item's placement by specifying the grid lines of a grid item's grid area.}}
{{CSS Property
|Initial value=auto
|Applies to=Grid items
|Inherited=No
|Media=visual
|Computed value=As specified
|Animatable=No
|CSS percentages=N/A
|Values={{CSS Property Value
|Data Type=auto
|Description=The property contributes nothing to the grid item’s placement.
}}{{CSS Property Value
|Data Type=<ident>
|Description=If there is a named grid area with the specified name, contributes a line to the placement by specifying the line at the corresponding edge of that named grid area. Otherwise, if there is a named line with the specified name, contributes a line to the placement by specifying the first line of that name. 
Otherwise, contributes nothing to the placement.
}}{{CSS Property Value
|Data Type=<integer> <ident>
|Description=Contributes a line to the placement by specifying the Nth grid line. (Negative integers are allowed, but zero is not; if <integer> is omitted, it defaults to 1.) If a name is given as an <ident>, only lines with that name are counted. If no line with that name exists, it instead specifies the first grid line (or the last, if <integer> is negative). If not enough lines of that name exist, it specifies the last such named line (or the first, if the <integer> is negative).
}}{{CSS Property Value
|Data Type=span [ <integer> | <ident> ]
|Description=Contributes a grid span to the placement by specifying that the corresponding edge of the item’s grid area is N grid lines from the opposite edge of the item's grid area. (Negative integers and zero are not allowed; if <integer> is omitted, it defaults to 1.) If a name is given as an <ident>, only lines with that name are counted. If no line with that name exists, the name is ignored. If not enough lines of that name exist, it spans to the last such named line.
}}
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Language=CSS
|Code=/* auto */
grid-row-start: auto

/* <ident> */
grid-row:start: "C";

/* <integer> <ident> */
grid-row:start: 2 "B";

/* span <integer> */
grid-row:start: span 2;

/* span <ident> */
grid-row:start: span "C";

}}
}}
{{Notes_Section}}
{{Related_Specifications_Section
|Specifications={{Related Specification
|Name=W3C Grid Layout Module
|URL=http://www.w3.org/TR/css3-grid-layout
|Status=W3C Working Draft
}}
}}
{{Compatibility_Section
|Not_required=No
|Imported_tables=
|Desktop_rows=
|Mobile_rows=
|Notes_rows=
}}
{{See_Also_Section}}
{{Topics|CSS}}
{{External_Attribution
|Is_CC-BY-SA=No
|MDN_link=
|MSDN_link=
|HTML5Rocks_link=
}}