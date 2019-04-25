---
title: singleValueLegacyExtendedProperty リソースの種類
description: '単一値が含まれる拡張プロパティ。 '
localization_priority: Normal
ms.openlocfilehash: 0d889756204853a525269f28cfdd3cc1b40be8a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523743"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>singleValueLegacyExtendedProperty リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

単一値が含まれる拡張プロパティ。 

オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | サポートされているリソースインスタンス: [message](../resources/message.md)、 [mailfolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactfolder](../resources/contactfolder.md)、 [outlook の仕事](../resources/outlooktask.md)、または[outlook のタスクフォルダー](../resources/outlooktaskfolder.md)。ただし、グループの[投稿](../resources/post.md)は含まれません。 | サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。 |
|[Get](../api/singlevaluelegacyextendedproperty-get.md) |サポートされているリソースインスタンス ([message](../resources/message.md)、 [mailfolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactfolder](../resources/contactfolder.md)、 [outlook タスク](../resources/outlooktask.md)、 [outlook タスクフォルダー](../resources/outlooktaskfolder.md)、またはグループ[投稿](../resources/post.md)) の1つまたは複数のコレクション。または、 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)オブジェクトを使用して展開されたインスタンスが1つあります。 |`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string|プロパティ識別子。読み取り専用です。|
|value|string|プロパティ値。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/singlevaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
