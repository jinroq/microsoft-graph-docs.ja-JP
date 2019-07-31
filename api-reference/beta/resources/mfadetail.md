---
title: mfaDetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3f38fae4d0360386592f956bee05d55738ad6910
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009665"
---
# <a name="mfadetail-resource-type"></a>mfaDetail リソースの種類
特定のサインインの MFA の詳細を示します。 これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。 



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|authDetail|String|MFA が必須である、対応するサインインアクティビティの MFA 認証詳細が "Yes" であることを示します。|
|authMethod|String|MFA 必須フィールドが "Yes" の場合に、対応するサインインアクティビティの MFA 認証方法 (SMS、Phone、Authenticator アプリ) を示します。|

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
