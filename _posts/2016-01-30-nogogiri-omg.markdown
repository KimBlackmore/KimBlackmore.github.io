---
layout: post
title:  "Well Hello Nokogiri"
date:   2016-01-30 09:00:00
categories: coding discoveries
---
Well I have discovered Nokogiri, thanks to Skillcush. OMG this is the most amazing thing. The answer to one of my most pressing problems. You see I have been in charge of establishing a course outline database at the [ANU][anu], called [Concourse][concourse], and the most annoying thing is trying to keep it in sync with the universities online handbook, [Programs and Courses][P&C].

[anu]: 			http://www.anu.edu.au/
[concourse]: 	https://anu.campusconcourse.com/search?search_performed=1&offset=0&sort_by=title&descend=false&plugin=item_report&report_format=html_tabular&selected_item_class=Syllabus&keyword=&advanced_performed=true&keyword_mode=all&title=&prefix=&number=&campus_id=3&school_id=-1&department_id=12&instructor=&session=&year=&credits=&delivery_method=&registration=_&template=_&timeframe=&audit_status=

[P&C]: 			http://programsandcourses.anu.edu.au/Search?Source=Catalogue&SearchText=&Search=&FiltersApplied=Courses&Careers%5B0%5D=&Careers%5B1%5D=&Careers%5B2%5D=&Careers%5B3%5D=&FilterByPrograms=false&FilterByCourses=true&FilterByMajors=false&FilterByMinors=false&FilterBySpecialisations=false&DegreeIdentifiers%5B0%5D=&DegreeIdentifiers%5B1%5D=&DegreeIdentifiers%5B2%5D=&Sessions%5B0%5D=&Sessions%5B1%5D=First+Semester&Sessions%5B2%5D=&Sessions%5B3%5D=&Sessions%5B4%5D=&Sessions%5B5%5D=&SelectedYear=2016&AtarMin=70.00&AtarMax=100.00&CollegeName=CAP

In particular, the course title, description, requisites, learning outcomes, number of units, and when it is offered need to match. There is no way to generate a report from P&C that can then be uploaded to Concourse. Instead, the administrators update P&C are supposed to email my group to let me know to make corresponding changes, but that is subject to process error. So, 18 months ago Chris who was working in my group and getting bored of manual Concourse updates suggested he write a web-scraper to extract this information from P&C and then it can be uploaded to Concourse automatically using feeds. Sounds like a dream, but Chris left without getting it done :-(. That was sad :-( But I had other assistance and we plugged away with manual updates, spot-checks, and responsive error corrections.

But now I can see that I will be able to create the web-scraper tool using nokogiri. Woo hoo! And just in time too as the group is disbanding and the replacement group will be too small for al this manual updating. If I can create the syncing tool I will talk to ITS about getting "someone" to own it and make sure it keeps running, and then we will have a system that the whole Uni will be able to get on and use. Hooray!


