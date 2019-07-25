---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3d5361bada5506bb04481711f47dd737db5d7f76
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856182"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReview accessReview = new AccessReview();
accessReview.displayName = "TestReview";
accessReview.startDateTime = "2017-02-10T00:35:53.214Z";
accessReview.endDateTime = "2017-03-12T00:35:53.214Z";
Identity reviewedEntity = new Identity();
reviewedEntity.id = "99025615-a0b1-47ec-9117-35377b10998b";
accessReview.reviewedEntity = reviewedEntity;
accessReview.reviewerType = "delegated";
accessReview.businessFlowTemplateId = "6e4f3d20-c5c3-407f-9695-8460952bcc68";
accessReview.description = "Sample description";
LinkedList<AccessReviewReviewer> reviewersList = new LinkedList<AccessReviewReviewer>();
AccessReviewReviewer reviewers = new AccessReviewReviewer();
reviewers.id = "f260246a-09b1-4fd5-8d18-daed736071ec";
reviewersList.add(reviewers);
AccessReviewReviewer reviewers1 = new AccessReviewReviewer();
reviewers1.id = "5a4e184c-4ee5-4883-96e9-b371f8da88e3";
reviewersList.add(reviewers1);
accessReview.reviewers = reviewersList;
AccessReviewSettings settings = new AccessReviewSettings();
settings.mailNotificationsEnabled = true;
settings.remindersEnabled = true;
settings.justificationRequiredOnApproval = true;
settings.autoReviewEnabled = false;
settings.activityDurationInDays = 30;
settings.autoApplyReviewResultsEnabled = false;
settings.accessRecommendationsEnabled = false;
AccessReviewRecurrenceSettings recurrenceSettings = new AccessReviewRecurrenceSettings();
recurrenceSettings.recurrenceType = "onetime";
recurrenceSettings.recurrenceEndType = "endBy";
recurrenceSettings.durationInDays = 0;
recurrenceSettings.recurrenceCount = 0;
settings.recurrenceSettings = recurrenceSettings;
AutoReviewSettings autoReviewSettings = new AutoReviewSettings();
autoReviewSettings.notReviewedResult = "Deny";
settings.autoReviewSettings = autoReviewSettings;
accessReview.settings = settings;

graphClient.accessReviews()
    .buildRequest()
    .post(accessReview);

```