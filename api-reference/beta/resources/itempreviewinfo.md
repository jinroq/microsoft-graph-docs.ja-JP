---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: itempreviewinfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: c43626292cd07ad14d27202255a499b413dbae63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345513"
---
# <a name="itempreviewinfo-resource-type"></a>itempreviewinfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itempreviewinfo**リソースには、[ドライブ項目](driveitem.md)のプレビューを埋め込む方法に関する情報が含まれています。

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
| posturl        | string | HTTP POST (form post、JS など) を使用した埋め込みに適した URL
| postparameters | string | posturl を使用する場合に含める POST パラメーター

指定したオプションの現在の状態に応じて、getUrl、posturl、または both のどちらかが返される場合があります。

postparameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。 例:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

url とパラメーターの形式は、不明瞭であると見なされます。
