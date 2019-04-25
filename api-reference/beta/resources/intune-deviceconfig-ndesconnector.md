---
title: ndesconnector リソースの種類
description: OnPrem Ndes コネクタを表すエンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3781827d93f1e646becc2ee47de57cbba82dfc63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554472"
---
# <a name="ndesconnector-resource-type"></a>ndesconnector リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

OnPrem Ndes コネクタを表すエンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ndesconnectors を一覧表示する](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)コレクション|[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ndesconnector の取得](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ndesconnector の作成](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|新しい[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。|
|[ndesconnector の削除](../api/intune-deviceconfig-ndesconnector-delete.md)|なし|[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)を削除します。|
|[ndesconnector の更新](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|NDES connector のキー。|
|lastConnectionDateTime|DateTimeOffset|Ndes connector の最終接続時刻|
|state|[ndesコネクタ状態](../resources/intune-deviceconfig-ndesconnectorstate.md)|Ndes connector の状態。 使用可能な値は、`none`、`active`、`inactive` です。|
|displayName|String|Ndes connector のフレンドリ名。|

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





