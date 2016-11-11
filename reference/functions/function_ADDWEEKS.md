---
title: "ADDWEEKS"
layout: "function"
isPage: "true"
link: "/warpscript/functions"
desc: "Adds a certain number of weeks to a timestamp."
categoryTree: ["reference","functions"]
category: "reference"
---
 

The `ADDWEEKS` function modifies a timestamp by adding a specified number of weeks to it. Optionally a timezone can be specified so the computation is performed using it instead of `UTC`.

Timezone names are the ones defined in [Joda Time](http://joda-time.sourceforge.net/timezones.html).

This function will take into account leap years and possible daylight saving time change.

## Example ##

{% raw %}
<warp10-warpscript-widget backend="{{backend}}"  exec-endpoint="{{execEndpoint}}">'2016-10-30T12:00:00Z' TOTIMESTAMP
'Europe/Paris' 1 ADDDAYS
'Europe/Paris' ISO8601
</warp10-warpscript-widget>
{% endraw %}        