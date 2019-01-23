---
title: windowsKioskAzureADGroup リソースの種類
description: キオスクの構成の AzureAD グループを識別するに使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4c8e0867346253c6501ebe8be490ba56800ab3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392571"
---
# <a name="windowskioskazureadgroup-resource-type"></a>windowsKioskAzureADGroup リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスクの構成の AzureAD グループを識別するに使用するクラス


[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|この構成にキオスクがロックアウトされている AzureAD グループの表示名|
|groupId|String|この構成にキオスクがロックアウトされている AzureAD グループの ID|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```




