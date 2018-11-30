---
title: 'driveItem: プレビュー'
description: このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。
ms.openlocfilehash: 741e449c972ad372aae30d9921cdb3b7fa1fc40d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023107"
---
# <a name="driveitem-preview"></a>driveItem: プレビュー

このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。

有効期間の長い埋め込みリンクを取得する場合は、 [createLink][] API を使用してください。

> **注:****プレビュー**の動作は、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)
|:---------------------------------------|:-------------------------------------------
| 委任 (職場または学校のアカウント)     | Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All
| 委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.ReadWrite.All
| アプリケーション                            | サポートされていません。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>要求本文

要求の本文では、アプリケーションが要求する埋め込み可能な URL のプロパティを定義します。
要求は、次のプロパティを含む JSON オブジェクトである必要があります。

|   名前      |  型         | 説明
|:------------|:--------------|:-----------------------------------------------
| page        | 文字列と番号 | 省略可能。 該当する場合に、開始するドキュメントのページ数です。 将来使用する場合は、ZIP などのファイルの種類を文字列として指定します。
| ズーム        | 数値        | 省略可能。 該当する場合に、開始するレベルを拡大します。

## <a name="response"></a>応答

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

応答は、次のプロパティを含む JSON オブジェクトになります。

| 名前           | 型   | 説明
|:---------------|:-------|:---------------------------------------------------
| getUrl         | 文字列 | HTTP の GET (iframe など) を使用して埋め込みの適切な URL
| postUrl        | 文字列 | HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。
| postParameters | 文字列 | PostUrl を使用する場合は、POST のパラメーター

GetUrl、postUrl、またはその両方は、指定したオプションの埋め込みのサポートの現在の状態によって返される可能性があります。

として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。 例:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>ページ/ズーム

'ページ' と '拡大' オプションは、すべてのプレビュー アプリケーションを使用できない場合がありますが、プレビュー アプリケーションでサポートされている場合に適用されます。
