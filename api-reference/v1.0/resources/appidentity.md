---
title: appIdentity リソースの種類
description: アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション Id、名前、サービスプリンシパル ID、名前が含まれます。 このリソースは、directoryAudit API によって呼び出されます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a8b2c9185f595bf4ab534dda5a73b1a5f40fd17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030094"
---
# <a name="appidentity-resource-type"></a>appIdentity リソースの種類

アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション ID、名前、およびサービスプリンシパル ID と名前が含まれます。 このリソースは、 [Get directoryAudit](../api/directoryaudit-get.md)操作で使用されます。

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|appId|String|Azure Active Directory でのアプリケーション ID を表す一意の GUID を参照します。|
|displayName|文字列|Azure Portal に表示されるアプリケーション名を参照します。|
|servicePrincipalId|String|対応するアプリの Azure Active Directory でサービスプリンシパル Id を示す一意の GUID を参照します。|
|servicePrincipalName|文字列型 (String)|サービスプリンシパル名がテナント内のアプリケーション名であることを示します。 |

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
