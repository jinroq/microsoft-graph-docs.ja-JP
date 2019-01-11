---
title: emailSyncSchedule 列挙型
description: 電子メールの同期スケジュールの可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838396"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





