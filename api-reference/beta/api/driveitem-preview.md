---
title: 'ドライブアイテム: プレビュー'
description: このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 74e6058d61fc5672bedd5e6479829f234707c45a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325150"
---
# <a name="driveitem-preview"></a>ドライブアイテム: プレビュー

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの url を取得できます。

長時間の埋め込み可能なリンクを取得する場合は、代わりに[createlink][] API を使用します。

> **注:** 現在、**プレビュー**アクションは SharePoint および OneDrive for business でのみ使用できます。

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)
|:---------------------------------------|:-------------------------------------------
| 委任 (職場または学校のアカウント)     | ファイル。読み取り、ファイルの読み取り/書き込み。すべてのファイル。
| 委任 (個人用 Microsoft アカウント) | ファイル。読み取り、ファイルの読み取り/書き込み。
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

要求の本文は、アプリケーションが要求している埋め込み可能な URL のプロパティを定義します。
要求は、次のプロパティを含む JSON オブジェクトである必要があります。

|   名前      |  型         | 説明
|:------------|:--------------|:-----------------------------------------------
| ビューアー      | string        | 省略可能。 使用するプレビューアプリ。 `onedrive` または `office`。 null の場合は、適切なビューアーが自動的に選択されます。
| chromeless  | ブール値       | 省略可能。 If `true` (既定値) の場合、埋め込まれたビューにコントロールは含まれません。
| allowEdit   | ブール値       | 省略可能。 の`true`場合は、埋め込み UI からファイルを編集できます。
| page        | 文字列または数値 | 省略可能。 開始するドキュメントのページ番号 (該当する場合)。 ZIP などのファイルの種類に関する今後のユースケースの文字列として指定されます。
| ズーム        | number        | 省略可能。 必要に応じて、開始するズームレベルを表示します。

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
| getUrl         | string | HTTP GET (iframes など) を使用した埋め込みに適した URL
| posturl        | string | HTTP POST (form post、JS など) を使用した埋め込みに適した URL
| postparameters | string | posturl を使用する場合に含める POST パラメーター

指定したオプションの embed サポートの現在の状態に応じて、getUrl、posturl、または both のどちらかが返される場合があります。

postparameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。 例:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>表示者

**viewer**パラメーターには次の値を使用できます。

| 種類の値 | 説明
|:-----------|:----------------------------------------------------------------
| null     | ファイルをレンダリングするための適切なアプリを選択します。 ほとんどの場合、これは`onedrive`プレビューアーを使用しますが、ファイルの種類によって異なる場合があります。
| `onedrive` | OneDrive プレビューアーアプリを使用して、ファイルをレンダリングします。
| `office`   | WAC (Office online) を使用して、ファイルをレンダリングします。 Office ドキュメントに対してのみ有効です。

### <a name="chrome-vs-chromeless"></a>クロム vs chromeless

が`chromeless` true の場合、プレビューはファイルのベア・レンダリングとなります。
それ以外の場合は、ドキュメント/ビューと対話するためのツールバー/ボタンが追加されている場合があります。

### <a name="viewedit"></a>表示/編集

が`allowEdit` true の場合、ドキュメントは、埋め込みプレビューでユーザーが操作することで変更できます。
この機能は、プレビューアプリやファイルの種類によっては使用できない場合があります。

### <a name="pagezoom"></a>ページ/ズーム

および`page` `zoom`オプションは、すべてのプレビューアプリで使用できるわけではありませんが、プレビューアプリがサポートしている場合は適用されます。
