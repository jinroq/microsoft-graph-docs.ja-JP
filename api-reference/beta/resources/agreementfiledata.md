---
title: agreementFileData リソースの種類
description: Azure Active Directory (Azure AD) 利用規約ファイルの blob を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: da4e600480e6ddd65112323b22f7a905b3ba29db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013424"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 利用規約ファイルの blob を表します。

## <a name="properties"></a>プロパティ
| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|data|Binary|使用条件を表すデータ。 PDF ドキュメント。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
