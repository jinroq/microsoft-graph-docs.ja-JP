---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420501"
---
# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings リソース タイプ

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

通知設定を記述するアイテムです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|bundleID|String|これらの通知設定を適用するアプリのバンドル ID。|
|appName|String|bundleID に関連するアプリケーション名。|
|publisher|String|bundleID に関連するパブリッシャー。|
|enabled|Boolean|通知がこのアプリで許可されているかどうかを示します。|
|showInNotificationCenter|Boolean|通知センターに通知を表示できるかどうかを示します。|
|showOnLockScreen|Boolean|ロック画面に通知を表示できるかどうかを示します。|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|このアプリの通知用の警告の種類を示します。 可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。|
|badgesEnabled|Boolean|バッジがこのアプリで許可されているかどうかを示します。|
|soundsEnabled|Boolean|サウンドがこのアプリで許可されているかどうかを示します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```




