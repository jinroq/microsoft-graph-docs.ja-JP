---
title: emailSyncSchedule 列挙型
description: 電子メールの同期スケジュールの可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425184"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メールの同期スケジュールの可能な値です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|asMessagesArrive|1|メッセージの受信時に同期します。|
|手動|2|手動で同期します。|
|fifteenMinutes|3|15 分ごとの同期します。|
|thirtyMinutes|4|30 分ごとの同期します。|
|sixtyMinutes|5|同期は 60 分ごと。|
|basedOnMyUsage|6|私の使用率に基づく同期。|




