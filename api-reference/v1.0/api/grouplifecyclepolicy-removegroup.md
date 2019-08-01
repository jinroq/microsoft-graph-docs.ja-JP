---
title: 'groupLifecyclePolicy: removeGroup'
description: ライフ サイクル ポリシーからグループを削除します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b6f5e7b736ad1467d9cdf0f20e9d5626b6d950c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014558"
---
# <a name="grouplifecyclepolicy-removegroup"></a>groupLifecyclePolicy: removeGroup

ライフ サイクル ポリシーからグループを削除します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---------------|:----------|
| Authorization | ベアラー {トークン}。必須。 |
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | 型 | 説明 |
|:---------------|:--------|:----------|
|groupId|Guid| ポリシーから削除するグループの ID です。|

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードを返します。 グループがポリシーから削除された場合、応答本体で、**true**値が返されます。 それ以外の場合、返信の本文で **false** 値が返されます。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a>応答
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
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
