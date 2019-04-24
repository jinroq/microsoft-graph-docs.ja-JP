---
title: governanceResource の登録
description: PIM に管理されていない governanceResource オブジェクトを登録します。
localization_priority: Normal
ms.openlocfilehash: f65c8b5884f08377967d3418bade0d5fc70c2063
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463951"
---
# <a name="register-governanceresource"></a>governanceResource の登録

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理されていない[governanceResource](../resources/governanceresource.md)オブジェクトを特権 id 管理に登録します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

>**注:** この API では、要求者がリソースに対して少なくとも1つのアクティブなロール割り当てを持っている必要もあります。

|アクセス許可の種類      | アクセス許可              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | PrivilegedAccess AzureResources  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | PrivilegedAccess AzureResources |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/resources/register
```

### <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッド**** は、応答`$select`を`$expand`カスタマイズするためのおよび[OData クエリパラメーター](/graph/query-parameters)のみをサポートしています。

### <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | Bearer {code}|
| Content-type  | application/json|

### <a name="request-body"></a>要求本文

|パラメーター      |Type                 |必須 |説明|
|:-------------|:----------------------|:--------|:----------|
|externalId    |String                 |✓        |PIM に登録するリソースの externalid。|

### <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答を返します。

### <a name="example"></a>例
この例では、Azure サブスクリプションの Wingtip Toys-生産を登録する方法を示します。
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a>要求
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/register
```
##### <a name="response"></a>応答
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-register.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
