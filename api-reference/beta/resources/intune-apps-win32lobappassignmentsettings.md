---
title: win32LobAppAssignmentSettings リソースの種類
description: Win32 の LOB のモバイル アプリケーションをグループに割り当てるために使用するプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 215b5c7086c2336f80bc0b812a108fbe2e2c1740
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430375"
---
# <a name="win32lobappassignmentsettings-resource-type"></a>win32LobAppAssignmentSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 の LOB のモバイル アプリケーションをグループに割り当てるために使用するプロパティが含まれています。


[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|通知|[win32LobAppNotification](../resources/intune-apps-win32lobappnotification.md)|通知の状態このアプリケーションの割り当て。 可能な値は、`showAll`、`showReboot`、`hideAll` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```




