---
title: 'driveItem: プレビュー'
description: このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508539"
---
# <a name="driveitem-preview"></a>driveItem: プレビュー

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| ビューアー      | string        | 省略可能。 使用するアプリケーションをプレビューします。 `onedrive` や `office` などになります。 Null の場合、適切なビューアーが自動的に選択されます。
| クロムレス  | boolean       | 省略可能。 場合`true`(既定値)、組み込みのビューのコントロールは含まれません。
| AllowEdit   | boolean       | 省略可能。 場合`true`、埋め込まれた UI からファイルを編集することができます。
| page        | 文字列と番号 | 省略可能。 該当する場合に、開始するドキュメントのページ数です。 将来使用する場合は、ZIP などのファイルの種類を文字列として指定します。
| ズーム        | number        | 省略可能。 該当する場合に、開始するレベルを拡大します。

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
| getUrl         | string | HTTP の GET (iframe など) を使用して埋め込みの適切な URL
| postUrl        | string | HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。
| postParameters | string | PostUrl を使用する場合は、POST のパラメーター

GetUrl、postUrl、またはその両方は、指定したオプションの埋め込みのサポートの現在の状態によって返される可能性があります。

として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。 次に例を示します。
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>ビューアー

**ビューアー**パラメーターには、次の値を指定します。

| 種類の値 | 説明
|:-----------|:----------------------------------------------------------------
| Null
     | ファイルを表示するための適切なアプリケーションを選択します。 使用するほとんどの場合、`onedrive`プレビューアーをファイルの種類によって異なる場合がありますが。
| `onedrive` | ファイルをレンダリングするのにには、OneDrive 対応のアプリケーションを使用します。
| `office`   | WAC (Office オンライン) を使用して、ファイルをレンダリングします。 Office ドキュメントに対してのみ有効です。

### <a name="chrome-vs-chromeless"></a>クロムレスのクロム vs

場合`chromeless`が true の場合、プレビュー、ファイルの最小限のレンダリングになります。
それ以外の場合、ドキュメント/ビューと対話するために表示されるその他のツールバーとボタンがある可能性があります。

### <a name="viewedit"></a>表示/編集

場合`allowEdit`が true の場合、埋め込まれたプレビューをユーザーの操作によって、ドキュメントを変更できます。
この機能は、すべてのプレビューのアプリケーションまたはファイルの種類のできない場合があります。

### <a name="pagezoom"></a>ページ/ズーム

`page`と`zoom`オプションは、すべてのプレビュー アプリケーションを使用できない場合がありますが、プレビューのアプリケーションをサポートしている場合に適用されます。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
