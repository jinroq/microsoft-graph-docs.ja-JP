---
title: 'ユーザー: exportpersonal data'
description: 組織のユーザーのデータをエクスポートするために、会社の管理者によって行われたデータポリシー操作要求を送信します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba26d2b2bc5af63f01a4333490d9850ffa3dd767
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576277"
---
# <a name="user-exportpersonaldata"></a>ユーザー: exportpersonal data

組織のユーザーのデータをエクスポートするために、会社の管理者またはアプリケーションからデータポリシー操作要求を送信します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  すべてのユーザーをエクスポートします。  |
|委任 (個人用 Microsoft アカウント) |  該当しない  |
|アプリケーション | すべてのユーザーをエクスポートします。 |

>**注:** エクスポートは、委任されたアクセス許可を使用する場合にのみ、会社の管理者が実行できます。

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}|

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|storagelocation|String|これは、データのエクスポート先となる Azure Storage アカウントの shared access signature (SAS) URL です。|

## <a name="response"></a>応答
成功した場合、このメソッドは `202 Accepted` 応答コードを返します。 応答本文には何も返されません。 応答には、次の応答ヘッダーが含まれています。

| 名前       | 説明|
|:---------------|:----------|
| Location  | 要求の状態を確認するための URL。 |
| 再試行-後  | 期間 (秒単位)。 要求を送信した後に、要求の状態を確認するための要求を送信する必要があります。 |

## <a name="example"></a>例
##### <a name="request"></a>要求
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a>応答

```
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
