---
title: deviceComplianceActionType 列挙型
description: スケジュールされたアクションの種類列挙
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05f9df39c563a47fa571a4badcf789ea4ddb08b1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979530"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

スケジュールされたアクションの種類列挙

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAction|.0|アクションなし|
|お知らせ|1-d|通知の送信|
|拒否|pbm-2|AAD でデバイスをブロックする|
|削除|1/3|デバイスをインベントリから削除する|
|ふき|2/4|デバイスをワイプする|
|removeResourceAccessProfiles|5|デバイスからリソースアクセスプロファイルを削除する|
|pushNotification|9 |デバイスへのプッシュ通知の送信|
|remoteLock|10 |デバイスをリモートでロックする|





