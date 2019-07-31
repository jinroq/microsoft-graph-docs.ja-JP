---
title: informationalUrl リソースの種類
description: アプリケーションの基本的なプロファイル情報です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e2eaad003f4669623a4db4af1b364e05198515d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006256"
---
# <a name="informationalurl-resource-type"></a>informationalUrl リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションの基本的なプロファイル情報です。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|市場|String| アプリケーションの [マーケティング] ページにリンクします。 たとえば、https://www.contoso.com/app/marketing のように指定します。 |
|秘密|String| アプリケーションのプライバシーに関する声明にリンクします。 たとえば、https://www.contoso.com/app/privacy のように指定します。 |
|・|String| アプリケーションのサポートページにリンクします。 たとえば、https://www.contoso.com/app/support のように指定します。 |
|termsOfService|String| アプリケーションのサービス条件ステートメントにリンクします。 たとえば、https://www.contoso.com/app/termsofservice のように指定します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
