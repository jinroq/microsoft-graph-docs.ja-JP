---
title: windowsmanagementapphealthstate リソースの種類
description: Windows management アプリの正常性状態エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c02904a5a4cc4d0242c35e487d30f2b2ed6083a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519999"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsmanagementapphealthstate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows management アプリの正常性状態エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション|[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsmanagementapphealthstate を取得する](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsmanagementapphealthstate を作成する](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|新しい[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。|
|[windowsmanagementapphealthstate の削除](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|なし|[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。|
|[windowsmanagementapphealthstate を更新する](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Windows management アプリの正常性状態の一意識別子|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows management アプリの正常性状態。 使用可能な値は、`unknown`、`healthy`、`unhealthy` です。|
|バージョン|String|Windows management アプリがインストールされているバージョン。|
|lastCheckInDateTime|DateTimeOffset|Windows management アプリの最終チェックイン時刻。|
|deviceName|String|Windows management アプリがインストールされているデバイスの名前。|
|deviceosversion|String|windows 管理アプリがインストールされているデバイスの windows 10 OS バージョン。|

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





