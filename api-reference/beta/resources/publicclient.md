---
title: publicClient リソースの種類
description: 以外の Web アプリケーションまたは Web Api の設定を指定します。 (モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644057"
---
# <a name="publicclient-resource-type"></a>publicClient リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以外の Web アプリケーションまたは Web Api の設定を指定します。 (モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|redirectUris|String コレクション| ユーザー トークンは、サインイン用に送信される Url または Uri を OAuth 2.0 の認証コードとアクセス トークンに送信のリダイレクトを指定します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
