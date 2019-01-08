---
title: 'ユーザー: exportPersonalData'
description: 組織のユーザーのデータをエクスポートするのには企業の管理者によって行われる、データ ポリシーの操作要求を送信します。
ms.openlocfilehash: 9308e955e83ccad5779d8261537306a5220d8086
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748214"
---
# <a name="user-exportpersonaldata"></a>ユーザー: exportPersonalData

企業の管理者または組織のユーザーのデータをエクスポートするのにはアプリケーションからのデータ ポリシー操作要求を送信します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |  User.Export.All、User.Read.All  |
|委任 (個人用 Microsoft アカウント) |  該当なし  |
|アプリケーション | User.Export.All、User.Read.All |

>**注:** 委任されたアクセス許可を使用すると、企業の管理者がエクスポートを実行のみできます。

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

| パラメーター    | 種類   |説明|
|:---------------|:--------|:----------|
|storageLocation|String|これは、データをエクスポートする必要があります、Azure ストレージ アカウントに共有アクセス署名 (SA) の URL です。|

## <a name="response"></a>応答
成功した場合、このメソッドは `202 Accepted` 応答コードを返します。 応答本体には何もは返されません。 応答には、次の応答ヘッダーが含まれています。

| 名前       | 説明|
|:---------------|:----------|
| Location  | 要求のステータスを確認する URL です。 |
| 再試行した後  | までの時間 (秒単位)。 要求のメーカーは、これを待つ必要があります後の状態をチェックする要求を送信します。 |

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
