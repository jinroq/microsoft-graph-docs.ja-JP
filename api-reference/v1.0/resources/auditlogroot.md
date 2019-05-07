---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 457fb3d7e67049d25ce02ea448a206b732d2175b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629335"
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
|directoryAudits|[Directoryaudit](directoryAudit.md)コレクション| 読み取り専用。 Null 許容型。|
|signIns|[サインイン](signIn.md)コレクション| 読み取り専用。Null 許容型です。|

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

<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```

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
  "tocPath": ""
}-->
