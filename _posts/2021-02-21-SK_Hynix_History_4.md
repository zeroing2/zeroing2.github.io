---
title: Firmware Static Analysis Process 셋업 & Static Analysis 자동화 In-House Tool 개발
categories: 
 - static analysis
 - process
 - automation
toc: true
---



1. ## Overview

![GitHub Logo](/assets/img/SK_Hynix_History_4/overview.PNG)

2. ## 과거

   개발중인 과제 코드에 대한 Static Analysis Process 가 존재하지 않았습니다.

   주기적으로 개발 과제 코드를 이용하여 Static Analysis를 수행할 인력이 없었고, 개발 Leader이 해당 Process의 중요도를 인식하지 못했습니다.

   외부 Audit 과 고객 Requirement에 Static Analysis가 명시됨에 따라 해당 Process의 중요도가 많이 높아졌습니다. 하지만, 공수가 많이 들고 많은 수동 작업이 필요했기 때문에, Process 를 셋팅하면서 자동화까지 고려해야 하는 상황이 발생했습니다.

3. ## 현재

   Static Analysis  Process가 성공적으로 셋업됐고, 많은 부분을 자동화시켰습니다.

   미국, 벨라루스, 한국 연구소에서 해당 Process를 사용하고 있으며, 해당 서비스를 3년동안 아무 문제없이 유지해오고 있습니다. 

   Process 를 셋업하면서 개발된 Automation Tool 은 Java를 기반으로 만들어졌으며, Issue Tracker Tool 인 JIRA의 REST API를 이용합니다. 해당 REST API를 통해 Static Analysis 에서 발견된 Defect 정보를 각 과제 개발 Leader에게 JIRA Ticket 을 발행하여 E-mail로 Noti 해주고 있습니다.

   Process의 모든 과정은 Log에 저장되며, 이를 기반으로 Audit을 대응하고 있습니다.  해당 Process는 외부 Consulting 업체를 통해 자문 받은결과, 현 시점에서 Samsung 보다 우위에 있다고 평가받았습니다.