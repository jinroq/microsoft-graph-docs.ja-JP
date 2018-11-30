---
title: audioRoutingGroup リソースの種類
description: オーディオのルーティング グループでは、通話参加者の間にプライベート オーディオ ルートを格納します。 ソースは参加者自身で、受信者、通話の他の参加者のサブセットであります。
ms.openlocfilehash: 98c58e39773567f13a2723e94c0413efd2841cd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066832"
---
# <a name="audioroutinggroup-resource-type"></a>audioRoutingGroup リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

オーディオのルーティング グループでは、通話参加者の間にプライベート オーディオ ルートを格納します。 ソースは参加者自身で、受信者、通話の他の参加者のサブセットであります。

> **注:**[ConfigureMixer](../api/participant-configuremixer.md)は、任意のルートを伴わないのすべての呼び出し元と受信者間の組み合わせのボリューム レベルを設定するためです。

## <a name="methods"></a>メソッド

| メソッド                                                  | 戻り値の型                               | 説明                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [AudioRoutingGroup を取得します。](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | AudioRoutingGroup オブジェクトのプロパティと関係を参照してください。|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | 受信者リストを更新します。                       |
| [削除](../api/audioroutinggroup-delete.md)            | なし                                      | オーディオのルーティング グループを削除します。              |

## <a name="properties"></a>プロパティ

| プロパティ      | 型              | 説明                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | 読み取り専用。 サーバーを生成します。                                         |
| 受信機     | 文字列コレクション | 参加者の id を受信する] ボックスの一覧です。                                   |
| routingMode   | String            | ルーティング グループのモードです。  使用可能な値は、`oneToOne`、`multicast` です。   |
| ソース       | 文字列コレクション | ソースの構成要素の id の一覧です。                                      |

> **注:** ルーティング モードでは、送信元と受信機の制限を決定します。 次のルーティング グループのみがサポートされています。
> - `oneToOne`-ソースと受信機に 1 つだけの参加者がそれぞれが含まれています。
> - `multicast`-ソース 1 人の参加者が複数の受信機があります。 受信者リストを更新する可能性があります。

> **注:** 多くのオーディオ ルーティング グループ (参加者ごとの bot など) を作成する場合は、4 最上位の優先度の高いスピーカーのオーディオのみが転送されます。 カスタマイズされたオーディオのルーティング グループを使用しても意味のスピーカーがおさまるように、メインのミキサーでない場合は、本人聞こえない bot でこのスピーカーと、bot のためだけのオーディオのプライベート グループがある場合でもします。

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
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
