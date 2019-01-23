---
title: configurationManagerClientEnabledFeatures リソースの種類
description: 構成マネージャーのクライアントに対応した機能
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425905"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

構成マネージャーのクライアントに対応した機能

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|inventory|Boolean|在庫が Intune によって管理されているかどうか|
|modernApps|Boolean|モダン アプリケーションが Intune によって管理されているかどうか|
|resourceAccess|Boolean|リソース アクセスが Intune によって管理されているかどうか|
|deviceConfiguration|Boolean|デバイス構成が Intune によって管理されているかどうか|
|compliancePolicy|Boolean|コンプライアンス ポリシーが Intune によって管理されているかどうか|
|windowsUpdateForBusiness|Boolean|Windows Update for Business が Intune によって管理されているかどうか|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```




