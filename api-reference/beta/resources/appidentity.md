---
title: appIdentity リソースの種類
description: アクションを実行するか、変更されているアプリケーションの id を示します。 アプリケーション Id、名、サービス ・ プリンシパルの ID および名前が含まれています。 このリソースは、directoryAudit API によって呼び出されます。
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855784"
---
# <a name="appidentity-resource-type"></a>appIdentity リソースの種類
アクションを実行するか、変更されているアプリケーションの id を示します。 アプリケーション Id、名、サービス ・ プリンシパルの ID および名前が含まれています。 このリソースは、 [directoryAudit](../api/directoryaudit-get.md) API によって呼び出されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|appId|文字列型 (String)|Azure Active Directory 内のアプリケーションの Id を表す一意の GUID を参照します。|
|displayName|String|Azure ポータルに表示されるアプリケーション名を参照します。|
|servicePrincipalId|String|Azure Active Directory 内のサービス ・ プリンシパルの Id を対応するアプリケーションを示す一意の GUID を参照します。|
|servicePrincipalName|文字列型 (String)|参照して、サービス プリンシパル名は、テナントにアプリケーションの名前です。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
