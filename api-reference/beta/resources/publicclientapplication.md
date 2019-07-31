---
title: publicClientApplication リソースの種類
description: 非 Web アプリまたは Web Api の設定を指定します。 (たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4503e65777b41fc2f864cd818697b048e3c8e435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965559"
---
# <a name="publicclientapplication-resource-type"></a>publicClientApplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

非 Web アプリまたは Web Api の設定を指定します。 (たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|redirectUris|文字列コレクション| サインインのためにユーザートークンが送信される Url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト Uri を指定します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
