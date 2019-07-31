---
title: emailSyncSchedule 列挙型
description: 電子メール同期スケジュールに指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 14b73fc4cfbf9cf53bdab4c2841403cac4077fa2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001426"
---
# <a name="emailsyncschedule-enum-type"></a>emailSyncSchedule 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

電子メール同期スケジュールに指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|Asメッセージの受信|1-d|メッセージが到着したときに同期します。|
|手動|pbm-2|手動で同期します。|
|fifteenMinutes|1/3|15分ごとに同期します。|
|thirtyMinutes|2/4|30分ごとに同期します。|
|sixtyMinutes|5|60分ごとに同期します。|
|basedOnMyUsage|シックス|自分の使用状況に基づいて同期します。|





