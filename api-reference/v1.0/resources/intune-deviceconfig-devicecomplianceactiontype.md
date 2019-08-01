---
title: deviceComplianceActionType 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cea72fa6e48699e540a43ea3938986e19ed351d3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028519"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 列挙型

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



