---
title: GovernanceRoleAssignmentRequests のエクスポート
description: ブラウザーで .csv ファイルとして解析`application/octet-stream`できる形式で governanceRoleAssignmentRequests のコレクションを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 227968ab265c117e5fa297d8fd8d8a988ddd0028
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954285"
---
# <a name="export-governanceroleassignmentrequests"></a>GovernanceRoleAssignmentRequests のエクスポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ブラウザーで .csv ファイル[](../resources/governanceroleassignmentrequest.md)として解析`application/octet-stream`できる形式で governanceRoleAssignmentRequests のコレクションを取得します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |


## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをリソースにエクスポートする
    
>**注:** この要求では、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てが必要になります。 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートする
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、型`application/octet-stream`のコンテンツを返します。

## <a name="example"></a>例
この例では、すべての役割の割り当てを、Wingtip Toys のサブスクリプションの .csv ファイルとして保存します。 

##### <a name="request"></a>要求
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>応答
以下は、応答の例です。 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
