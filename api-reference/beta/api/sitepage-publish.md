---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: '[発行] ページ'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e59a7aea74e165945757f2513102a66baf64be1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920241"
---
# <a name="sitepage-publish"></a>sitePage: 発行

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ページのバージョンをすべてのユーザーが使用可能にする[sitePage][]リソースの最新バージョンを公開します。 ページがチェック アウトされている場合は、ページをチェックインし、公開します。 この API の呼び出し元ページがチェック アウトされた場合ページが自動的にチェックインし、公開します。

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a>要求本文

このメッセージには、要求の本体がありません。 送信の要求の本文は無視されます。

## <a name="response"></a>応答

成功すると、API 呼び出しは `204 No Content` を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
