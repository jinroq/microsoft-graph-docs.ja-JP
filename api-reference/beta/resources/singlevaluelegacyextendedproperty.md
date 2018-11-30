---
title: singleValueLegacyExtendedProperty リソースの種類
description: '単一値が含まれる拡張プロパティ。 '
ms.openlocfilehash: 1b9eeaa05ee15aab30c1761cd35f70f586dffb24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073323"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>singleValueLegacyExtendedProperty リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

単一値が含まれる拡張プロパティ。 

オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | サポートされているリソース インスタンス:[メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook の仕事](../resources/outlooktask.md)または[Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、ですが、グループに[投稿](../resources/post.md)がありません。 | サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。 |
|[Get](../api/singlevaluelegacyextendedproperty-get.md) |([メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md) [Outlook の仕事](../resources/outlooktask.md)、 [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、またはグループの[転記](../resources/post.md))、サポートされているリソースのインスタンスのコレクションの 1 つまたはまたは、このような 1 つのインスタンスは、 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)オブジェクトを使用して展開します。 |`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ID|string|プロパティ識別子。読み取り専用です。|
|value|文字列|プロパティ値。|

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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->