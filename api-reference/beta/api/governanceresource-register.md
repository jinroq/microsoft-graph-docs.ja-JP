---
title: 'governanceResource: register'
description: PIM に governanceResource オブジェクトを登録します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b8457f7ddee4564ca6b6b300121ddb7b8247e34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713920"
---
# <a name="governanceresource-register"></a>governanceResource: register

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特権 Id 管理に[governanceResource](../resources/governanceresource.md)オブジェクトを登録します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** この API では、要求者がリソースに対して少なくとも1つのアクティブなロール割り当てを持っている必要もあります。

| アクセス許可の種類 | アクセス許可 |
|:--------------- |:----------- |
| 委任 (職場または学校のアカウント) | PrivilegedAccess AzureResources |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッド**** は、応答`$select`を`$expand`カスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)のみをサポートしています。

## <a name="request-headers"></a>要求ヘッダー

| 名前 | 説明 |
|:---- |:----------- |
| Authorization | ベアラー {トークン} |
| Content-type | application/json |

## <a name="request-body"></a>要求本文

| プロパティ | 型 | 説明 |
|:---------- |:---- |:----------- |
| externalId | String | PIM に登録するリソースの外部識別子。 サブスクリプションを登録する場合、識別子はサブスクリプション id の先頭に`/subscriptions/`になります。 たとえば、`/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac` などです。 |

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答を返します。

## <a name="example"></a>例

次の例は、この API を呼び出す方法を示しています。
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
Content-type: application/json

{
  "externalId": "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"
}
```
### <a name="response"></a>応答
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Register governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
