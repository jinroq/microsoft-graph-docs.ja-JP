---
title: ndesConnector リソースの種類
description: Ndes の OnPrem コネクタを表すエンティティです。
author: tfitzmac
ms.openlocfilehash: e37a20c440546094424d0284bd1d7ffbbeb60bdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332292"
---
# <a name="ndesconnector-resource-type"></a>ndesConnector リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Ndes の OnPrem コネクタを表すエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を一覧表示します。|
|[NdesConnector を取得します。](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を参照してください。|
|[NdesConnector を作成します。](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。|
|[NdesConnector を削除します。](../api/intune-deviceconfig-ndesconnector-delete.md)|なし|の[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)を削除します。|
|[NdesConnector を更新します。](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|NDES のコネクタのキー。|
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





