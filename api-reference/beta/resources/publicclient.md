---
title: publicClient リソースの種類
description: 以外の Web アプリケーションまたは Web Api の設定を指定します。 (モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)
localization_priority: Normal
ms.openlocfilehash: c466c91f90ac8adc2bf3806fa212e0b01e6d2507
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864198"
---
# <a name="publicclient-resource-type"></a>publicClient リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

以外の Web アプリケーションまたは Web Api の設定を指定します。 (モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
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
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
