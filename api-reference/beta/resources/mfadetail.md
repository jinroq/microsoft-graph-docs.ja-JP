---
title: mfaDetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 サインインで認証の詳細と、使用する認証方法が含まれています (例: 電話、SMS、またはボイス メール) '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883742"
---
# <a name="mfadetail-resource-type"></a>mfaDetail リソースの種類
特定のサインインの MFA の詳細を示します。 サインインで認証の詳細と、使用する認証方法が含まれています (例: 電話、SMS、またはボイス メール) 



## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|authDetail|String|必要な MFA は、[はい] とは、対応する記号の活動の MFA の認証の詳細を示します。|
|authMethod|String|MFA のために必要なフィールドは、[はい] をするときに、対応する記号の活動の MFA の認証方法 (SMS、電話、ユーザー認証システムのアプリケーションは、いくつかの値) を示します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
