---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c43367465ac89116fcdca2460deb832d2cfbe746
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444023"
---
# <a name="auditlogroot-resource-type"></a>auditLogRoot リソースの種類

さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[directoryAudits を一覧表示する](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。|
|[directoryAudit を取得する](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |特定のディレクトリの監査アイテムとそのプロパティを取得します。|
|[サインインを一覧表示する](../api/signin-list.md) | [サインイン](signin.md) |サインイン オブジェクトのプロパティとリレーションシップを読み取ります。|
|[サインインを取得する](../api/signin-get.md) | [サインイン](signin.md) |サインイン オブジェクトのプロパティとリレーションシップを読み取ります。|

## <a name="properties"></a>プロパティ

なし

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|directoryAudits|[Directoryaudit](directoryaudit.md)コレクション| 読み取り専用です。 Null 許容型。|
|signIns|[サインイン](signin.md)コレクション| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a>例


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
