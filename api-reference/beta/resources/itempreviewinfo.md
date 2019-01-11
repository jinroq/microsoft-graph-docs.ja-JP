---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
localization_priority: Normal
ms.openlocfilehash: 0f2a161b9b43a8d372b90530b1b9d9244f77d8e9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857345"
---
# <a name="itempreviewinfo-resource-type"></a>ItemPreviewInfo リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**ItemPreviewInfo**リソースには、 [DriveItem](driveitem.md)のプレビューを埋め込む方法についての情報が含まれています。

## <a name="json-representation"></a>JSON 表記

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>プロパティ

| 名前           | 種類   | 説明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | 文字列 | HTTP の GET (iframe など) を使用して埋め込みの適切な URL
| postUrl        | 文字列 | HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。
| postParameters | 文字列 | PostUrl を使用する場合は、POST のパラメーター

GetUrl、postUrl、またはその両方は、指定したオプションのサポートの現在の状態によって返される可能性があります。

として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。 次に例を示します。
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

不透明な Url とパラメーターの形式を検討してください。
