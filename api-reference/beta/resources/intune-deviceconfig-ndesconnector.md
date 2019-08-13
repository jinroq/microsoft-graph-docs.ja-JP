---
title: ndesConnector リソースの種類
description: OnPrem Ndes コネクタを表すエンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00608f053d5c41d25a089708165af7494cf435d2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368626"
---
# <a name="ndesconnector-resource-type"></a>ndesConnector リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

OnPrem Ndes コネクタを表すエンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[NdesConnectors を一覧表示する](../api/intune-deviceconfig-ndesconnector-list.md)|[Ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション|[Ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[NdesConnector の取得](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[Ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[NdesConnector の作成](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|新しい[Ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。|
|[NdesConnector の削除](../api/intune-deviceconfig-ndesconnector-delete.md)|None|[Ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)を削除します。|
|[NdesConnector の更新](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[Ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|NDES Connector のキー。|
|lastConnectionDateTime|DateTimeOffset|Ndes Connector の最終接続時刻|
|state|[Ndesコネクタ状態](../resources/intune-deviceconfig-ndesconnectorstate.md)|Ndes Connector の状態。 可能な値は、`none`、`active`、`inactive` です。|
|displayName|String|Ndes Connector のフレンドリ名。|

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



