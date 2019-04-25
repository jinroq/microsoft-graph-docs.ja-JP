---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: SharePoint サイトからページを削除する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537115"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>サイトのサイトページリストからページを削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[サイト][]のサイトページ[リスト][]から[sitepage][]を削除します。

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[サイト]: ../resources/site.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前       | 値 | 説明
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a>応答

成功した場合、この呼び出し`204 No Content`は、リソースが削除され、戻り値がないことを示す応答を返します。

## <a name="example"></a>例

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a>要求

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a>応答

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
