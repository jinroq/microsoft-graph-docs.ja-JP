---
title: dataPolicyOperation リソースの種類
description: 送信されたデータポリシー操作を表します。 操作の状態を追跡するために必要な情報が含まれています。 たとえば、会社の管理者は、従業員の会社のデータをエクスポートするためのデータポリシー操作要求を送信し、後でその要求を追跡できます。
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c73bef8a640c950b6d85eb74ad93089aaad4f74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029555"
---
# <a name="datapolicyoperation-resource-type"></a>dataPolicyOperation リソースの種類

送信されたデータポリシー操作を表します。 操作の状態を追跡するために必要な情報が含まれています。 たとえば、会社の管理者は、従業員の会社のデータをエクスポートするためのデータポリシー操作要求を送信し、後でその要求を追跡できます。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[DataPolicyOperation を取得する](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |**DataPolicyOperation**オブジェクトのプロパティを取得します。|
|[個人データをエクスポートする](../api/user-exportpersonaldata.md) | None |データポリシー操作要求を送信します。組織ユーザーのデータをエクスポートするには、後で[Get dataPolicyOperation](../api/datapolicyoperation-get.md)を使用して読み取ることができます。|

## <a name="properties"></a>プロパティ

> **注:** このリソースのすべてのプロパティは読み取り専用です。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|CompletedDateTime|DateTimeOffset|このデータポリシー操作の要求が完了すると、ISO 8601 形式を使用して UTC 時刻であることを表します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 操作が完了するまで Null 値を返します。|
|id|文字列| この操作の一意のキーです。 |
|status|string| 可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。|
|storageLocation|String|エクスポート要求のためにデータがエクスポートされる場所の URL。|
|userId|String|操作が実行されるユーザーの id。|
|submittedDateTime|DateTimeOffset|このデータ操作の要求が送信された時点 (UTC 時間) を表す ISO 8601 形式を使用します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|progress|String|操作の進行状況を指定します。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
