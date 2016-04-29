+++
date = "2016-04-28T19:58:21Z"
description = "Testing MathJax Mathematical Typesetting in Hugo"
draft = true
tags = []
title = "MathJax Test"
topics = []
+++

## This is some content

This is content.

`$ E = mc^2 $`

`$N_AN_D$`

Here's a tweet!
{{< tweet 63623585020915713 >}}

Here's a YouTube video: 
{{< youtube IvUU8joBb1Q >}}

And a vimeo video!
{{< vimeo 157712307 >}}


``` python
from time import localtime

activities = {8: 'Sleeping',
              9: 'Commuting',
              17: 'Working',
              18: 'Commuting',
              20: 'Eating',
              22: 'Resting' }

time_now = localtime()
hour = time_now.tm_hour

for activity_time in sorted(activities.keys()):
    if hour < activity_time:
        print activities[activity_time]
        break
else:
    print 'Unknown, AFK or sleeping!'
```


{{< highlight html >}}
<section id="main">
  <div>
    <h1 id="title">{{ .Title }}</h1>
    {{ range .Data.Pages }}
      {{ .Render "summary"}}
    {{ end }}
  </div>
</section>
{{< /highlight >}}
