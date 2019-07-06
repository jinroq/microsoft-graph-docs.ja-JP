---
title: riskDetection リソースの種類
description: AzureAD テナントのすべてのリスクの検出を表します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 07a3a76f2ec2a4c3e1536f4b4d61e52417c2053c
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576467"
---
# <a name="riskdetection-resource-type"></a>riskDetection リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD テナントの検出されたリスクに関する情報を表します。 

Azure AD は、さまざまなシグナルやマシン学習に基づいて、[ユーザーのリスク](riskyuser.md)とアプリまたはユーザー[のサインイン](signin.md)リスクを継続的に評価します。 この API は、Azure AD 環境のすべてのリスク検出へのプログラムによるアクセスを提供します。

リスクイベントの詳細については、「 [Azure Active Directory Id 保護](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)」を参照してください。

>[!NOTE]
>リスク検出 API を使用するには、Azure AD Premium P2 ライセンスが必要です。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リスト riskDetection](../api/riskdetection-list.md) | [riskDetection](riskdetection.md)コレクション|リスクの検出とそのプロパティを一覧表示します。|
|[RiskDetection を取得する](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|特定の危険な検出とそのプロパティを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|`id`|`string`|リスク検出の一意の ID。 |
|`requestId`|`string`|リスクの検出に関連付けられているサインインの要求 ID。 リスクの検出がサインインに関連付けられていない場合、このプロパティは null になります。|
|`correlationId`|`string`|リスクの検出に関連付けられているサインインの関連付け ID。 リスクの検出がサインインに関連付けられていない場合、このプロパティは null になります。 |
|`riskType`|`riskEventType`|検出されたリスクイベントの種類。 使用可能な値は、unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、、、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、Mcasimwait トラベル、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、および Unknownfuturevalue という。 |
|`riskState`|`riskState`|検出されたリスクの高いユーザーまたはサインインの状態。 使用可能な値は、none、confirmedSafe、修復、消さ、atRisk、confirmedCompromised、および Unknownfuturevalue というです。 |
|`riskLevel`|`riskLevel`|検出されたリスクのレベル。 使用可能な値は、low、medium、high、hidden、none、Unknownfuturevalue というです。 |
|`riskDetail`|`riskDetail`|検出されたリスクの詳細。 使用可能な値は、none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、Unknownfuturevalue という。 |
|`source`|`string`|リスク検出のソース。 たとえば、"activeDirectory" を使用します。 |
|`detectionTimingType`|`riskDetectionTimingType`|検出されたリスクのタイミング (リアルタイム/オフライン)。 指定可能な値は、定義されていません。リアルタイム、nearRealtime、offline、Unknownfuturevalue というです。 |
|`activity`|`activityType`|検出されたリスクがリンクされているアクティビティの種類を示します。 使用可能な値は、サインイン、ユーザー、Unknownfuturevalue というです。 |
|`tokenIssuerType`|`tokenIssuerType`|検出されたサインインリスクのトークン発行元の種類を示します。 使用可能な値は、AzureAD、ADFederationServices、および Unknownfuturevalue というです。 |
|`ipAddress`|`string`|リスクが発生したクライアントの IP アドレスを提供します。 |
|`location`|[`signInLocation`](signinlocation.md)|サインインの場所。 |
|`activityDateTime`|`datetimeoffset`|危険な活動が発生した日時。 |
|`detectedDateTime`|`datetimeoffset`|リスクが検出された日時。 |
|`lastUpdatedDateTime`|`datetime`|リスク検出が最後に更新された日付と時刻。 |
|`userId`|`string`|ユーザーの一意の ID。 |
|`userDisplayName`|`string`|ユーザーの名前 |
|`userPrincipalName`|`string`|ユーザーのユーザープリンシパル名 (UPN)。 |
|`additionalInfo`|`string`|JSON 形式でのリスクの検出に関連付けられている追加情報。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
