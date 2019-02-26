---
title: iosNotificationSettings リソース タイプ
description: 通知設定を記述するアイテムです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2876146e7e20ad94a7356f623a5b2e17443a18f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172703"
---
# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings リソース タイプ

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

通知設定を記述するアイテムです。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|bundleID|String|これらの通知設定を適用するアプリのバンドル ID。|
|appName|String|bundleID に関連するアプリケーション名。|
|publisher|String|bundleID に関連するパブリッシャー。|
|enabled|ブール型|通知がこのアプリで許可されているかどうかを示します。|
|showInNotificationCenter|Boolean|通知センターに通知を表示できるかどうかを示します。|
|showOnLockScreen|Boolean|ロック画面に通知を表示できるかどうかを示します。|
|alertType|[iosnotificationalerttype](../resources/intune-deviceconfig-iosnotificationalerttype.md)|このアプリの通知用の警告の種類を示します。 可能な値は、`deviceDefault`、`banner`、`modal`、`none` です。|
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




