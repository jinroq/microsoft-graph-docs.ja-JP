---
title: privilegedApproval リソースの種類
description: ロールを取得するために特権 Id 管理で要求される承認を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e920d34cc9a42c29138a97a83786087c86b7ee10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008916"
---
# <a name="privilegedapproval-resource-type"></a>privilegedApproval リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ロールを取得するために特権 Id 管理で要求される承認を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[privilegedApproval を取得する](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |PrivilegedApproval オブジェクトのプロパティとリレーションシップを読み取ります。|
|[PrivilegedApproval オブジェクトを一覧表示する](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) コレクション|PrivilegedApproval のコレクションを取得します。|
|[privilegedApproval を作成する](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |privilegedApproval オブジェクトを作成します。 |
|[privilegedApproval を更新する](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |privilegedApproval オブジェクトを更新します。 |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|リクエスターの承認要求を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|approvalDuration|期間||
|approvalState|string| 可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。|
|approvalType|String||
|approverReason|String||
|endDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String| 読み取り専用です。|
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|userId|String||

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 読み取り専用です。 Null 許容型。|
|タキ|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| 読み取り専用です。 この承認オブジェクトの役割の割り当て要求|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
