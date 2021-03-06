---
title: "m"
layout: "function"
isPage: "true"
link: "/warpscript/functions"
desc: "Convert a timestamp expressed in minutes to the time unit used by the platform"
categoryTree: ["reference","functions"]
category: "reference"
---
 

The `m` function consumes a timestamp expressed in minutes from the top of the stack and pushes back its conversion in the time unit used by the platform.

## Example ##

WarpScript commands:

    1 m

Stack: 

    TOP: 60000000 // If the platform is configured with microsecond as the time unit


{% raw %}
<warp10-warpscript-widget backend="{{backend}}"  exec-endpoint="{{execEndpoint}}">1 m
</warp10-warpscript-widget>
{% endraw %}    


## Unit test ##

{% raw %}
<warp10-warpscript-widget backend="{{backend}}"  exec-endpoint="{{execEndpoint}}">1 m
60 STU * == ASSERT
'unit test successful'
</warp10-warpscript-widget>
{% endraw %}        
