---
title: appidentity リソースの種類
description: アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション Id、名前、サービスプリンシパル Id、名前が含まれます。 このリソースは、directoryaudit API によって呼び出されます。
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535677"
---
# <a name="appidentity-resource-type"></a>appidentity リソースの種類
アクションを実行した、または変更されたアプリケーションの id を示します。 アプリケーション Id、名前、サービスプリンシパル Id、名前が含まれます。 このリソースは、 [directoryaudit](../api/directoryaudit-get.md) API によって呼び出されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|appId|String|Azure Active Directory でのアプリケーション ID を表す一意の GUID を参照します。|
|displayName|String|Azure Portal に表示されるアプリケーション名を参照します。|
|servicePrincipalId|String|対応するアプリの Azure Active Directory でサービスプリンシパル Id を示す一意の GUID を参照します。|
|servicePrincipalName|String|サービスプリンシパル名がテナント内のアプリケーション名であることを示します。 |

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
