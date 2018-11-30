---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022646"
---
# <a name="itempreviewinfo-resource-type"></a>itemPreviewInfo リソースの種類

**ItemPreviewInfo**リソースには、 [driveItem](driveitem.md)のプレビューを埋め込む方法についての情報が含まれています。

## <a name="json-representation"></a>JSON 表記

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>プロパティ

| 名前           | 型   | 説明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | 文字列 | HTTP の GET (iframe など) を使用して埋め込みの適切な URL
| postUrl        | 文字列 | HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。
| postParameters | 文字列 | PostUrl を使用する場合は、POST のパラメーター

GetUrl、postUrl、またはその両方は、指定したオプションのサポートの現在の状態によって返される可能性があります。

として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。 例:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

不透明な Url とパラメーターの形式を検討してください。
