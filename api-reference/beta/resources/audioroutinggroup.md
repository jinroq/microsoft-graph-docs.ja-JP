---
title: audioRoutingGroup リソースの種類
description: 音声ルーティンググループでは、複数の参加者の間のプライベートオーディオルートをマルチパーティの会話に格納します。 Source は参加者であり、受信者はマルチパーティの会話の他の参加者のサブセットです。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544002"
---
# <a name="audioroutinggroup-resource-type"></a>audioRoutingGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

音声ルーティンググループでは、複数の参加者の間のプライベートオーディオルートをマルチパーティの会話に格納します。 Source は参加者であり、受信者はマルチパーティの会話の他の参加者のサブセットです。

> **注:**[ConfigureMixer](../api/participant-configuremixer.md)には、すべてのルートは含まれません。送信元と受信側の組み合わせにボリュームレベルを設定するための呼び出し全体に対して使用されます。

## <a name="methods"></a>メソッド

| メソッド                                                  | 戻り値の型                               | 説明                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [audioRoutingGroup を取得する](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | audioRoutingGroup オブジェクトのプロパティとリレーションシップを読み取ります。|
| [更新](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | 受信者の一覧を更新します。                       |
| [削除](../api/audioroutinggroup-delete.md)            | なし                                      | オーディオルーティンググループを削除します。              |

## <a name="properties"></a>プロパティ

| プロパティ      | 型              | 説明                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | 読み取り専用です。 サーバーによって生成されます。                                         |
| 配信     | String コレクション | 受信側参加者 id のリスト。                                   |
| routingmode   | String            | ルーティンググループモード。  可能な値は、`oneToOne`、`multicast` です。   |
| sources       | String コレクション | ソース参加者 id のリスト。                                      |

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
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
