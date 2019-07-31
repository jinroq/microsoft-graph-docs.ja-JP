---
author: rahmit
description: SitePage リソースの最新バージョンを発行します。これにより、すべてのユーザーがページのバージョンを使用できるようになります。 ページがチェックアウトされている場合は、ページをチェックインして発行します。 ページがこの API の呼び出し元にチェックアウトされている場合、ページは自動的にチェックインされてから発行されます。
ms.date: 09/10/2018
title: ページの発行
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5f4404b33a54979271750d4074a9c6da235966ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991213"
---
# <a name="sitepage-publish"></a>サイトページ: 発行

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Sitepage][]リソースの最新バージョンを発行します。これにより、すべてのユーザーがページのバージョンを使用できるようになります。 ページがチェックアウトされている場合は、ページをチェックインして発行します。 ページがこの API の呼び出し元にチェックアウトされている場合、ページは自動的にチェックインされてから発行されます。

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

このメッセージには、要求本文がありません。 送信された要求本文は無視されます。

## <a name="response"></a>応答

成功すると、API 呼び出しは `204 No Content` を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->
