---
title: windowsManagementAppHealthSummary リソースの種類
description: Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 5717f96cbac534f2726ccf7bcfcbdb54d4c17b28
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326230"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a>windowsManagementAppHealthSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 管理アプリケーションの健康状態の概要のプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsManagementAppHealthSummary を取得します。](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsManagementAppHealthSummary を更新します。](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)|[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|Windows 管理アプリケーションの稼働状態の概要エンティティのキーです。|
|healthyDeviceCount|Int32|正常なデバイスの数。|
|unhealthyDeviceCount|Int32|問題のあるデバイスの数。|
|unknownDeviceCount|Int32|不明なデバイスの数。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```





