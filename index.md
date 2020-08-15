---

layout: col-sidebar
title: OWASP Nashua
tags: nashua
level: 0

region: North America
meetup-group: OWASP-Nashua-Chapter
country: USA
postal-code: 3060

---

## Welcome
Welcome to the Nashua, New Hampshire chapter!  

## Participation
The Open Web Application Security Project (OWASP) is a nonprofit foundation that works to improve the security of software. All of our projects, tools, documents, forums, and chapters are free and open to anyone interested in improving application security. 

Chapters are led by local leaders in accordance with the [Chapter Leader Handbook](/www-policy/rules-of-procedure/chapter-handbook). Financial contributions should only be made online using the authorized online donation button. To be a SPEAKER at ANY OWASP Chapter in the world simply review the [speaker agreement](/www-policy/speaker-agreement) and then contact the local chapter leader with details of what OWASP Project, independent research, or related software security topic you would like to present.

Everyone is welcome and encouraged to participate in our [Projects](/projects), [Local Chapters](/chapters), [Events](/events), [Online Groups](https://groups.google.com/a/owasp.com/){:target='_blank'}, and [Community Slack Channel](https://owasp.slack.com/){:target='_blank'}. We especially encourage diversity in all our initiatives. OWASP is a fantastic place to learn about application security, to network, and even to build your reputation as an expert. We also encourage you to be [become a member](/membership) or consider a [donation](/donate) to support our ongoing work.

## Local News
- Our local meetings are now virtual due to the pandemic.  You can get information by joining our [Meetup](https://www.meetup.com/OWASP-Nashua-Chapter/).
- Everyone is welcome to join us at our chapter meetings.

### Check our Upcoming Meetup Events:
{% include chapter_events.html group=page.meetup-group %}

<script type='text/javascript'>
  $(function(){
    $(".timeclass").hover(function() {
      utc_str = $(this).text();
      ndx = utc_str.indexOf(':');
      st_hour_str = utc_str.substring(0, ndx);
      st_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(st_hour_str), parseInt(st_min_str), 0);
      start_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);

      ndx = utc_str.lastIndexOf(':');
      end_hour_str = utc_str.substring(ndx - 2, ndx - 1);
      end_min_str = utc_str.substring(ndx + 1, ndx + 3);
      utc_dt = luxon.DateTime.utc(2020, 06, 06, parseInt(end_hour_str), parseInt(end_min_str), 0);
      end_dt = utc_dt.setZone(luxon.DateTime.local().zoneName);
      popstr = start_dt.toLocaleString(luxon.DateTime.TIME_WITH_SECONDS) + ' to ' + end_dt.toLocaleString(luxon.DateTime.TIME_WITH_SHORT_OFFSET);
      $(this).prop('title', popstr);
    });
  });
