---
title: windowsManagementAppHealthState リソースの種類
description: Windows 管理アプリケーションの正常性の状態エンティティです。
author: tfitzmac
ms.openlocfilehash: 5ff77ce54a99ed71a8f4b3498a469342b2e46367
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359704"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>windowsManagementAppHealthState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 管理アプリケーションの正常性の状態エンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsManagementAppHealthState を取得します。](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsManagementAppHealthState を作成します。](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|新しい[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。|
|[WindowsManagementAppHealthState を削除します。](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|なし|の[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。|
|[WindowsManagementAppHealthState を更新します。](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|Windows 管理アプリケーションの正常性状態の一意の識別子|
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





