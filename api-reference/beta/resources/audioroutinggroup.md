---
title: audioRoutingGroup リソースの種類
description: 音声ルーティンググループでは、複数の参加者の間のプライベートオーディオルートをマルチパーティの会話に格納します。 Source は参加者であり、受信者はマルチパーティの会話の他の参加者のサブセットです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: db5f94f9ac500dfeb97c6eb787783e9f749ae507
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974277"
---
# <a name="audioroutinggroup-resource-type"></a>audioRoutingGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

音声ルーティンググループでは、複数の参加者の間のプライベートオーディオルートをマルチパーティの会話に格納します。 Source は参加者であり、受信者はマルチパーティの会話の他の参加者のサブセットです。

> **注:**[ConfigureMixer](../api/participant-configuremixer.md)には、すべてのルートは含まれません。送信元と受信側の組み合わせにボリュームレベルを設定するための呼び出し全体に対して使用されます。

## <a name="methods"></a>メソッド

| メソッド                                                  | 戻り値の型                               | 説明                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [AudioRoutingGroup を取得する](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | AudioRoutingGroup オブジェクトのプロパティとリレーションシップを読み取ります。|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | 受信者の一覧を更新します。                       |
| [Delete](../api/audioroutinggroup-delete.md)            | None                                      | オーディオルーティンググループを削除します。              |

## <a name="properties"></a>プロパティ

| プロパティ      | 型              | 説明                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | string            | 読み取り専用です。 サーバーによって生成されます。                                         |
| 配信     | collection(string) | 受信側参加者 id のリスト。                                   |
| routingMode   | string            | ルーティンググループモード。  可能な値は、`oneToOne`、`multicast` です。   |
| sources       | collection(string) | ソース参加者 id のリスト。                                      |

> **注:** ルーティングモードは、送信元と受信者に対する制限を決定します。 次のルーティンググループのみがサポートされています。
> - `oneToOne`-ソースと受信者には、それぞれ1人の参加者のみが含まれます。
> - `multicast`-ソースには1つの参加者がいますが、複数の受信者がいます。 受信者の一覧が更新された可能性があります。

> **注:** 多数のオーディオルーティンググループ (参加者ごとに bot など) を作成する場合は、上位4台の主要なスピーカーのオーディオのみが転送されます。 カスタマイズされたオーディオルーティンググループを使用している場合でも、メインミキサーでスピーカーの音量が十分でない場合は、このスピーカーと bot のみに専用のオーディオグループがある場合でも、そのユーザーは bot によって聞くことはできません。

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
