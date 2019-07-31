---
title: synchronizationSecretKeyStringValuePair リソースの種類
description: '1つのシークレット値を表します。 '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad3348cea31567cedfca9b2626c81383ab8c6b8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964700"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a>synchronizationSecretKeyStringValuePair リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

1つのシークレット値を表します。 

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Key|String| 可能な値: `None`、 `UserName` `Password` `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain`、、、、、、、、、、、、 `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.|
|value|文字列型 (String)|シークレットの値。|

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
