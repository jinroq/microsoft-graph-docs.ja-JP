---
title: privilegedApproval リソースの種類
description: 要求された特権 Id 管理の役割に承認を表します。
localization_priority: Normal
ms.openlocfilehash: dee8cffba02270308c6786b2549b66aa5ad9dfa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868349"
---
# <a name="privilegedapproval-resource-type"></a>privilegedApproval リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

要求された特権 Id 管理の役割に承認を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[PrivilegedApproval を取得します。](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |PrivilegedApproval オブジェクトのプロパティと関係を参照してください。|
|[PrivilegedApproval オブジェクトのリスト](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md)コレクション|PrivilegedApproval のコレクションを取得します。|
|[PrivilegedApproval を作成します。](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |PrivilegedApproval オブジェクトを作成します。 |
|[PrivilegedApproval を更新します。](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |PrivilegedApproval オブジェクトを更新します。 |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|要求側の承認の要求を取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|approvalDuration|Duration||
|approvalState|文字列| 可能な値は、`pending`、`approved`、`denied`、`aborted`、`canceled` です。|
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
|roleInfo|[privilegedRole](privilegedrole.md)| 読み取り専用。Null 許容型。|
|要求|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| 読み取り専用です。 この承認オブジェクトのロール割り当ての依頼|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
