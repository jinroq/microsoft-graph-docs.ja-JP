---
title: レポート リソースの種類
description: Intune は、複数のワークフローをサポートする Microsoft グラフ API のレポートのリソースについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 098c20b2460324c4975533902e1b71fde1af41c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407474"
---
# <a name="report-resource-type"></a>レポート リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

コンテキストに適切なコンテンツを返すなど。

- デバイス構成のプロファイルの履歴のレポートです。
- 障害レポートを登録します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|content|Stream|レポート コンテンツです。詳細は、レポートの種類によって異なります。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



