---
title: '同期ジョブ: validateCredentials'
description: テナントで資格情報が有効であることを検証します。
localization_priority: Normal
ms.openlocfilehash: 4be9317f753865fdb956e58566ec1302d1542de5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330090"
---
# <a name="synchronizationjob-validatecredentials"></a>同期ジョブ: validateCredentials

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントで資格情報が有効であることを検証します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     |Directory.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |サポートされていません。 |
|アプリケーション                            |サポートされていません。| 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター    | 型   |説明|
|:---------------|:--------|:----------|
|の場合は、資格情報|Boolean|の`true`場合、 `credentials`パラメーターは無視され、以前に保存された資格情報 (ある場合) が代わりに検証されます。 |
|クリデンシャル|[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)コレクション|検証する資格情報。 `useSavedCredentials`パラメーターがの場合は`true`無視されます。|

## <a name="response"></a>応答
検証が成功した場合、このメソッド`204, No Content`は応答コードを返します。 応答本文には何も返されません。

## <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```

##### <a name="response"></a>応答
応答の例を次に示します。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
