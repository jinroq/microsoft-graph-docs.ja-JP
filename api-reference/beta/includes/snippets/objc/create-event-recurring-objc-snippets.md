---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 36045d6121808fbcd475511bc1d69df1ae5c946b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723975"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEvent *event = [[MSGraphEvent alloc] init];
[event setSubject:@"Let's go for lunch"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Does noon time work for you?"];
[event setBody:body];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2017-09-04T12:00:00"];
[start setTimeZone:@"Pacific Standard Time"];
[event setStart:start];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2017-09-04T14:00:00"];
[end setTimeZone:@"Pacific Standard Time"];
[event setEnd:end];
MSGraphPatternedRecurrence *recurrence = [[MSGraphPatternedRecurrence alloc] init];
MSGraphRecurrencePattern *pattern = [[MSGraphRecurrencePattern alloc] init];
[pattern setType: [MSGraphRecurrencePatternType weekly]];
[pattern setInterval: 1];
NSMutableArray *daysOfWeekList = [[NSMutableArray alloc] init];
[daysOfWeekList addObject: @"Monday"];
[pattern setDaysOfWeek:daysOfWeekList];
[recurrence setPattern:pattern];
MSGraphRecurrenceRange *range = [[MSGraphRecurrenceRange alloc] init];
[range setType: [MSGraphRecurrenceRangeType endDate]];
[range setStartDate:@"2017-09-04"];
[range setEndDate:@"2017-12-31"];
[recurrence setRange:range];
[event setRecurrence:recurrence];
MSGraphLocation *location = [[MSGraphLocation alloc] init];
[location setDisplayName:@"Harry's Bar"];
[event setLocation:location];
NSMutableArray *attendeesList = [[NSMutableArray alloc] init];
MSGraphAttendee *attendees = [[MSGraphAttendee alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"AdeleV@contoso.onmicrosoft.com"];
[emailAddress setName:@"Adele Vance"];
[attendees setEmailAddress:emailAddress];
[attendees setType: [MSGraphAttendeeType required]];
[attendeesList addObject: attendees];
[event setAttendees:attendeesList];

NSError *error;
NSData *eventData = [event getSerializedDataWithError:&error];
[urlRequest setHTTPBody:eventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```