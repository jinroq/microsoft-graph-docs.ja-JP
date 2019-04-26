---
title: skypeforbusinessactivityuserdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: e847cbf469db3be55c8c12ebf31056a262962886
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571766"
---
# <a name="skypeforbusinessactivityuserdetail-resource-type"></a>skypeforbusinessactivityuserdetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                                 | 型              |
| :--------------------------------------- | :---------------- |
| totalPeerToPeerSessionCount              | Int64             |
| totalOrganizedConferenceCount            | Int64             |
| totalParticipatedConferenceCount         | Int64             |
| peertopeerlastactivitydate               | Date              |
| organizedConferenceLastActivityDate      | Date              |
| participatedConferenceLastActivityDate   | Date              |
| peertopeerimcount                        | Int64             |
| peertopeeraudiocount                     | Int64             |
| peertopeeraudiominutes                   | Int64             |
| peertopeervideocount                     | Int64             |
| peertopeervideominutes                   | Int64             |
| peertopeerappsharingcount                | Int64             |
| peertopeerfiletransfercount              | Int64             |
| organizedConferenceIMCount               | Int64             |
| organizedConferenceAudioVideoCount       | Int64             |
| organizedConferenceAudioVideoMinutes     | Int64             |
| organizedConferenceAppSharingCount       | Int64             |
| organizedConferenceWebCount              | Int64             |
| organizedConferenceDialInOut3rdPartyCount | Int64             |
| organizedConferenceCloudDialInOutMicrosoftCount | Int64             |
| organizedConferenceCloudDialInMicrosoftMinutes | Int64             |
| organizedConferenceCloudDialOutMicrosoftMinutes | Int64             |
| participatedConferenceIMCount           | Int64             |
| participatedConferenceAudioVideoCount   | Int64             |
| participatedConferenceAudioVideoMinutes | Int64             |
| participatedConferenceAppSharingCount   | Int64             |
| participatedConferenceWebCount          | Int64             |
| participatedConferenceDialInOut3rdPartyCount | Int64             |
| reportrefreshdate                        | Date              |
| userPrincipalName                        | String            |
| isDeleted                                | Boolean           |
| deletedDate                              | Date              |
| lastactivitydate                         | Date              |
| assignedProducts                         | String collection |
| reportperiod                             | String            |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```json
{
  "totalPeerToPeerSessionCount": 1024, 
  "totalOrganizedConferenceCount": 1024, 
  "totalParticipatedConferenceCount": 1024, 
  "peerToPeerLastActivityDate": "Date", 
  "organizedConferenceLastActivityDate": "Date", 
  "participatedConferenceLastActivityDate": "Date", 
  "peerToPeerIMCount": 1024, 
  "peerToPeerAudioCount": 1024, 
  "peerToPeerAudioMinutes": 1024, 
  "peerToPeerVideoCount": 1024, 
  "peerToPeerVideoMinutes": 1024, 
  "peerToPeerAppSharingCount": 1024, 
  "peerToPeerFileTransferCount": 1024, 
  "organizedConferenceIMCount": 1024, 
  "organizedConferenceAudioVideoCount": 1024, 
  "organizedConferenceAudioVideoMinutes": 1024, 
  "organizedConferenceAppSharingCount": 1024, 
  "organizedConferenceWebCount": 1024, 
  "organizedConferenceDialInOut3rdPartyCount": 1024, 
  "organizedConferenceCloudDialInOutMicrosoftCount": 1024, 
  "organizedConferenceCloudDialInMicrosoftMinutes": 1024, 
  "organizedConferenceCloudDialOutMicrosoftMinutes": 1024, 
  "participatedConferenceIMCount": 1024, 
  "participatedConferenceAudioVideoCount": 1024, 
  "participatedConferenceAudioVideoMinutes": 1024, 
  "participatedConferenceAppSharingCount": 1024, 
  "participatedConferenceWebCount": 1024, 
  "participatedConferenceDialInOut3rdPartyCount": 1024, 
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
