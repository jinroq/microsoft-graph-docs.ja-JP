---
title: androidKeyguardFeature 列挙型
description: Android keyguard 機能です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430342"
---
# <a name="androidkeyguardfeature-enum-type"></a>androidKeyguardFeature 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android keyguard 機能です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|次のように構成されません。この値は無視されます。|
|カメラ|1|セキュリティで保護された keyguard の画面上にあるときのカメラの使用法です。|
|通知|2|セキュリティで保護された keyguard の画面上にあるときの通知を表示しています。|
|unredactedNotifications|3|表示 unredacted、セキュリティで保護された keyguard の画面上にあるときに通知します。|
|trustAgents|4|セキュリティで保護された keyguard の画面上にあるとき、エージェントの状態を信頼します。|
|指紋|5|セキュリティで保護された keyguard の画面上にあるときのセンサーの使用状況を指紋します。|
|remoteInput|6|セキュリティで保護された keyguard の画面上にあるときの通知テキストを入力します。|
|allFeatures|7|セキュリティで保護された keyguard の画面上にあるとき、すべての keyguard 機能。|




