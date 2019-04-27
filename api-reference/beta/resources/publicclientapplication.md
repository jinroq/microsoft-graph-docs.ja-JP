---
title: publicclientapplication リソースの種類
description: 非 web アプリまたは web Api の設定を指定します。 (たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)
localization_priority: Normal
ms.openlocfilehash: 8118d1e771cb55ce5b82c9ddac14aaa45260ab56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348869"
---
# <a name="publicclientapplication-resource-type"></a>publicclientapplication リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

非 web アプリまたは web Api の設定を指定します。 (たとえば、デスクトップデバイス上で実行されているインストール済みアプリケーションなどの、モバイルまたはその他のパブリッククライアント)

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|redirecturis|String collection| サインインのためにユーザートークンが送信される url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト uri を指定します。 |

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
