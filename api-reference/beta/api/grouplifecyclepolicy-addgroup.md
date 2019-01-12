---
title: 'groupLifecyclePolicy: addGroup'
description: ライフ サイクル ポリシーにグループを追加します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3909d7a25a49c95e80041a4a708a5b8e823e0c91
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926625"
---
# <a name="grouplifecyclepolicy-addgroup"></a>groupLifecyclePolicy: addGroup

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ライフ サイクル ポリシーにグループを追加します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません |
|アプリケーション | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---------------|:----------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | Type | 説明 |
|:---------------|:--------|:----------|
|groupId|Guid| ポリシーに追加するグループの ID です。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードを返します。 グループがポリシーに追加された場合、応答本体で、**true** 値が返されます。 それ以外の場合、返信の本文で **false** 値が返されます。

## <a name="example"></a>例

#### <a name="request"></a>要求

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a>応答
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
