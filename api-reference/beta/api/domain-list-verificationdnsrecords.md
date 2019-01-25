---
title: verificationDnsRecords を一覧表示する
description: domainDnsRecord オブジェクトの一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a470f6bddb9cade8083afb3eb5d5cf76cf4dba32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522841"
---
# <a name="list-verificationdnsrecords"></a>verificationDnsRecords を一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトの一覧を取得します。

所有権を検証しないと、関連するドメインを Azure AD テナントで使用することはできません。ドメインの所有権を検証するには、ドメイン検証レコードを取得し、ドメインのゾーン ファイルに詳細を追加します。この作業は、ドメイン レジストラーによって、または DNS サーバーの構成で行えます。

ルート ドメインには検証が必要です。たとえば、contoso.com には検証が必要です。ルート ドメインが検証されると、ルート ドメインのサブドメインが自動的に検証されます。たとえば、contoso.com が検証されると、subdomain.contoso.com が自動的に検証されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.Read.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.Read.All、Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> {Id} には、ドメインを完全修飾ドメイン名で指定します。

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |
| Content-Type  | application/json |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domainDnsRecord](../resources/domaindnsrecord.md) オブジェクトのコレクションを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a>応答

注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-verificationdnsrecords.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
