---
title: informationalUrl リソースの種類
description: アプリケーションの基本的なプロファイル情報です。
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071532"
---
# <a name="informationalurl-resource-type"></a>informationalUrl リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーションの基本的なプロファイル情報です。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|マーケティング|String| アプリケーションのマーケティングのページにリンクします。 たとえば、https://www.contoso.com/app/marketing では、 |
|プライバシー|String| アプリケーションのプライバシーに関する声明へのリンクです。 たとえば、https://www.contoso.com/app/privacy では、 |
|サポート|String| アプリケーションのサポートのページにリンクします。 たとえば、https://www.contoso.com/app/support では、 |
|termsOfService|String| サービスのステートメントのアプリケーションの条件にリンクします。 たとえば、https://www.contoso.com/app/termsofservice では、 |

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
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->