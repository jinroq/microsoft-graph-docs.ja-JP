---
title: automaticRepliesSetting リソースの種類
description: '受信メールの送信者にメッセージを自動的に通知するための構成設定 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cad76eb9ebbd8646e96cea1b98cb8d87c20a3b23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030038"
---
# <a name="automaticrepliessetting-resource-type"></a>automaticRepliesSetting リソースの種類

サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。たとえば、サインイン ユーザーが電子メールに返信できないことを通知する自動返信などです。 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|externalAudience|externalAudienceScope| **Status** が **** または `AlwaysEnabled` の場合に、`Scheduled` を受信する、サインイン ユーザーの組織外の一連の対象ユーザー。 使用可能な値: `none`、`contactsOnly`、`all`。|
|externalReplyMessage|string|**Status** が `AlwaysEnabled` または `Scheduled` の場合、指定の外部対象ユーザーに送信される自動応答。|
|internalReplyMessage|string|**Status** が `AlwaysEnabled` または `Scheduled` の場合、サインイン ユーザーの組織内の対象ユーザーに送信される自動応答。 |
|scheduledEndDateTime|[dateTimeTimeZone](datetimetimezone.md)|**Status** が `Scheduled` に設定されている場合に、自動応答を終了する日時。 |
|scheduledStartDateTime|[dateTimeTimeZone](datetimetimezone.md)|**Status** が `Scheduled` に設定されている場合に、自動応答を開始する日時。|
|status|automaticRepliesStatus|自動応答の構成状態。 使用可能な値: `disabled`、`alwaysEnabled`、`scheduled`。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
