---
title: windowsManagementAppHealthState リソースの種類
description: Windows management アプリの正常性状態エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b443c95b363e926777150013e20bef4bc8bc602d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942172"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsManagementAppHealthState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows management アプリの正常性状態エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション|[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsManagementAppHealthState を取得する](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsManagementAppHealthState を作成する](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|新しい[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。|
|[WindowsManagementAppHealthState の削除](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|None|[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。|
|[WindowsManagementAppHealthState を更新する](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Windows management アプリの正常性状態の一意識別子|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows management アプリの正常性状態。 可能な値は、`unknown`、`healthy`、`unhealthy` です。|
|バージョン|String|Windows management アプリがインストールされているバージョン。|
|lastCheckInDateTime|DateTimeOffset|Windows management アプリの最終チェックイン時刻。|
|deviceName|String|Windows management アプリがインストールされているデバイスの名前。|
|deviceOSVersion|String|Windows 管理アプリがインストールされているデバイスの Windows 10 OS バージョン。|

## <a name="relationships"></a>関係
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




