---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e21a0eaf628580b197188dc46b26cb09b357bcf7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637745"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReview = {
    displayName:"TestReview",
    startDateTime:"2017-02-10T00:35:53.214Z",
    endDateTime:"2017-03-12T00:35:53.214Z",
    reviewedEntity: {
        id: "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    businessFlowTemplateId: "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    description:"Sample description",
    reviewers:
    [
        {
            id:"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            id:"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    settings:
    {
        mailNotificationsEnabled: true,
        remindersEnabled: true,
        justificationRequiredOnApproval:true,
        autoReviewEnabled:false,
        activityDurationInDays:30,
        autoApplyReviewResultsEnabled:false,
        accessRecommendationsEnabled:false,
        recurrenceSettings:{
            recurrenceType:"onetime",
            recurrenceEndType:"endBy",
            durationInDays:0,
            recurrenceCount:0
        },
        autoReviewSettings:{
            notReviewedResult:"Deny"
        }
    }
};

let res = await client.api('/accessReviews')
    .version('beta')
    .post(accessReview);

```