---
title: windowsManagementAppHealthState リソースの種類
description: Windows 管理アプリケーションの正常性の状態エンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 171ae2492eb5077567f4398af678d14044a0b7e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395735"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsManagementAppHealthState リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 管理アプリケーションの正常性の状態エンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsManagementAppHealthState を取得します。](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsManagementAppHealthState を作成します。](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|新しい[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。|
|[WindowsManagementAppHealthState を削除します。](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|なし|の[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。|
|[WindowsManagementAppHealthState を更新します。](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Windows 管理アプリケーションの正常性状態の一意の識別子|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows 管理アプリケーションの正常性状態。 可能な値は、`unknown`、`healthy`、`unhealthy` です。|
|installedVersion|String|Windows 管理アプリケーションは、バージョンをインストールします。|
|lastCheckInDateTime|DateTimeOffset|Windows 管理アプリケーション最後のチェックインの時間です。|
|deviceName|String|Windows 管理アプリケーションがインストールされているデバイスの名前です。|
|deviceOSVersion|String|Windows 管理アプリケーションがインストールされているデバイスの 10 の Windows OS のバージョンです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```




