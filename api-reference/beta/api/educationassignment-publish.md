---
title: 'educationAssignment: 発行'
description: この操作では、公開済みのステータスに、元のドラフト状態から、割り当ての状態を変更します。 クラスの先生だけでは、この呼び出しを行うことができます。 割り当ては、下書きの状態では、受講者は、割り当ては表示されませんも、提出書類の任意のオブジェクトになります。 この API を呼び出すときは、送信オブジェクトは作成され、割り当ては、受講者のリストに表示されます。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: c7cdaebb91490270cc0a8f205b41a89b662a7a13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926702"
---
# <a name="educationassignment-publish"></a>educationAssignment: 発行

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

この操作では、公開済みのステータスに、元のドラフト状態から、割り当ての状態を変更します。 クラスの先生だけでは、この呼び出しを行うことができます。 割り当ては、下書きの状態では、受講者は、割り当ては表示されませんも、提出書類の任意のオブジェクトになります。 この API を呼び出すときは、送信オブジェクトは作成され、割り当ては、受講者のリストに表示されます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | サポートされていません。 | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
次の例は、この API を呼び出す方法を示しています。
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a>応答
応答の例を次に示します。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
