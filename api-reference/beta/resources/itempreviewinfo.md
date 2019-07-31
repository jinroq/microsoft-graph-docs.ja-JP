---
author: kevinlam
description: ItemPreviewInfo リソースには、ドライブ項目のプレビューを埋め込む方法に関する情報が含まれています。
ms.date: 3/16/2018
title: ItemPreviewInfo-OneDrive API
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 2d789dacb0f1c1d3daca988f334fca2e8da4b0d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010057"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Itempreviewinfo**リソースには、[ドライブ項目](driveitem.md)のプレビューを埋め込む方法に関する情報が含まれています。

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
| getUrl         | string | HTTP GET (iframes など) を使用した埋め込みに適した URL
| postUrl        | string | HTTP POST (form post、JS など) を使用した埋め込みに適した URL
| postParameters | string | PostUrl を使用する場合に含める POST パラメーター

指定したオプションの現在の状態に応じて、getUrl、postUrl、または both のどちらかが返される場合があります。

postParameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。 次に例を示します。
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Url とパラメーターの形式は、不明瞭であると見なされます。
