---
title: 同期テンプレートを取得する
description: その識別子で同期テンプレートを取得します。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ef1c33422b36e8fd88fcc6646506905e2a091e1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991101"
---
# <a name="get-synchronizationtemplate"></a>同期テンプレートを取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

その識別子で同期テンプレートを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     |Directory.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |サポートされていません。|
|アプリケーション                            |サポートされていません。| 

### <a name="http-request"></a>HTTP 要求

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 型    | 説明|
|:---------------|:--------|:-----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

### <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期テンプレート](../resources/synchronization-synchronizationtemplate.md)オブジェクトを返します。

### <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a>応答
応答の例を次に示します。
>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しでは、すべてのプロパティが返されます。

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
