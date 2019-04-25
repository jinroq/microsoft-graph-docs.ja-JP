---
title: 'ドライブアイテム: プレビュー'
description: このアクションを使用すると、一時的なプレビューを表示するために、短時間に埋め込まれた、アイテムの url を取得できます。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572704"
---
# <a name="driveitem-preview"></a>ドライブアイテム: プレビュー

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

postparameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。 次に例を示します。
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>ページ/ズーム

[ページ] と [ズーム] オプションは、すべてのプレビューアプリで使用できるわけではありませんが、プレビューアプリがサポートしている場合は適用されます。
