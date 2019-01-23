---
title: windowsUniversalAppXAppAssignmentSettings リソースの種類
description: Windows ユニバーサル AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27755a483be44584aeb82166f56e825df79f8eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400719"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a>windowsUniversalAppXAppAssignmentSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ユニバーサル AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。


[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|useDeviceContext|ブール型 (Boolean)|Windows ユニバーサル AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```




