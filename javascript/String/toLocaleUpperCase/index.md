{{Page_Title}}
{{Flags
|State=Ready to Use
|Editorial notes=
|Checked_Out=No
}}
{{Summary_Section|Returns a string where all alphabetic characters have been converted to uppercase, taking into account the host environment's current locale.}}
{{JS_Syntax
|Formats={{JS Syntax Format
|Format=stringVar.toLocaleUpperCase( )
}}
|Values=
}}
{{JS_Return_Value
|Description=
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Language=JavaScript
|Description=
|Code=var hello = "wOrLd";
var foobar = hello.toLocaleUpperCase();
console.log(hello); // "wOrLd"
console.log(foobar); // "WORLD"
|LiveURL=
}}
}}
{{Remarks_Section
|Remarks=The required stringVar reference is a String object or string literal.

The '''toLocaleUpperCase''' method converts the characters in a string, taking into account the host environment's current locale. In most cases, the result is the same as the result the '''toUpperCase''' method. Results differ if the rules for a language conflict with the regular Unicode case mappings, such as Turkish.
}}
{{Notes_Section
|Usage=
|Notes=
|Import_Notes=
}}
{{JS Object Listing}}
{{Topics | JS Basic}}
{{See_Also_Section
|Manual_links=* [[javascript/String/toLocaleLowerCase{{!}}toLocaleLowerCase Method (String)]]
* [[javascript/String/toUpperCase{{!}}toUpperCase Method (String)]]
|External_links=
|Manual_sections=
}}
{{JS Topics
|JS Page Type=JS Basic
|Applies to=
}}
{{External_Attribution
|Is_CC-BY-SA=No
|Sources=MSDN
|MDN_link=
|MSDN_link=http://msdn.microsoft.com/en-us/library/ie/6t6xaca8(v=vs.94).aspx
|HTML5Rocks_link=
}}