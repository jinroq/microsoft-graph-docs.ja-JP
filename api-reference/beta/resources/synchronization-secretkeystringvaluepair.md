---
title: synchronizationSecretKeyStringValuePair リソースの種類
description: '1 つの秘密の値を表します。 '
ms.openlocfilehash: 31aa5d983a0117591d3be75939b2c881a9782e7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073994"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a>synchronizationSecretKeyStringValuePair リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

1 つの秘密の値を表します。 

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Key|String| 使用可能な値: `None`、 `UserName`、 `Password`、 `SecretToken`、 `AppKey`、 `BaseAddress`、 `ClientIdentifier`、 `ClientSecret`、 `SingleSignOnType`、 `Sandbox`、 `Url`、 `Domain`、 `ConsumerKey`、 `ConsumerSecret`、 `TokenKey`、 `TokenExpiration`、 `Oauth2AccessToken`、 `Oauth2AccessTokenCreationTime`、 `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.|
|value|文字列|シークレットの値です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->