---
title: mfaDetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 サインインで認証の詳細と、使用する認証方法が含まれています (例: 電話、SMS、またはボイス メール) '
ms.openlocfilehash: a377c8648ebc8a6e3eb10fb6b0b87df066f8f2cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069753"
---
# <a name="mfadetail-resource-type"></a>mfaDetail リソースの種類
特定のサインインの MFA の詳細を示します。 サインインで認証の詳細と、使用する認証方法が含まれています (例: 電話、SMS、またはボイス メール) 



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
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