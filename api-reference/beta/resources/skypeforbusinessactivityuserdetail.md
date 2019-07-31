---
title: skypeForBusinessActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bd17deab26b061f48f762bf8ffeb5f8289b2a51f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008195"
---
# <a name="skypeforbusinessactivityuserdetail-resource-type"></a>skypeForBusinessActivityUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                                 | 型              |
| :--------------------------------------- | :---------------- |
| totalPeerToPeerSessionCount              | Int64             |
| totalOrganizedConferenceCount            | Int64             |
| totalParticipatedConferenceCount         | Int64             |
| peerToPeerLastActivityDate               | 日付              |
| organizedConferenceLastActivityDate      | 日付              |
| participatedConferenceLastActivityDate   | 日付              |
| peerToPeerIMCount                        | Int64             |
| peerToPeerAudioCount                     | Int64             |
| peerToPeerAudioMinutes                   | Int64             |
| peerToPeerVideoCount                     | Int64             |
| peerToPeerVideoMinutes                   | Int64             |
| peerToPeerAppSharingCount                | Int64             |
| peerToPeerFileTransferCount              | Int64             |
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
| reportRefreshDate                        | 日付              |
| userPrincipalName                        | String            |
| isDeleted                                | Boolean           |
| deletedDate                              | 日付              |
| lastActivityDate                         | 日付              |
| assignedProducts                         | 文字列コレクション |
| reportPeriod                             | String            |

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
