---
title: ndesConnector リソースの種類
description: Ndes の OnPrem コネクタを表すエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b504173c0a56e15fd2a4ba09ce50beeabbb20edc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411149"
---
# <a name="ndesconnector-resource-type"></a>ndesConnector リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Ndes の OnPrem コネクタを表すエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を一覧表示します。|
|[NdesConnector を取得します。](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を参照してください。|
|[NdesConnector を作成します。](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。|
|[NdesConnector を削除します。](../api/intune-deviceconfig-ndesconnector-delete.md)|なし|の[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)を削除します。|
|[NdesConnector を更新します。](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|NDES のコネクタのキー。|
|lastConnectionDateTime|DateTimeOffset|Ndes コネクタの前回の接続|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Ndes のコネクタの状態です。 可能な値は、`none`、`active`、`inactive` です。|
|displayName|String|Ndes のコネクタの表示名。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```




