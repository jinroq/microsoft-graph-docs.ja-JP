---
title: mfadetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。 '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581479"
---
# <a name="mfadetail-resource-type"></a>mfadetail リソースの種類
特定のサインインの MFA の詳細を示します。 これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。 



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|authdetail|String|mfa が必須である、対応するサインインアクティビティの mfa 認証詳細が "Yes" であることを示します。|
|authmethod|String|mfa 必須フィールドが "Yes" の場合に、対応するサインインアクティビティの mfa 認証方法 (SMS、Phone、Authenticator アプリ) を示します。|

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
