---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d824f579787bf24cc56704a1c8a9df280d969809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173508"
---
# <a name="devicecomplianceactiontype-enum-type"></a>devicecomplianceactiontype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

スケジュールされたアクションの種類列挙

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAction|.0|アクションなし|
|お知らせ|1-d|通知の送信|
|拒否|pbm-2|AAD でデバイスをブロックする|
|削除|1/3|デバイスをインベントリから削除する|
|ふき|2/4|デバイスをワイプする|
|removeresourceaccessprofiles|5|デバイスからリソースアクセスプロファイルを削除する|
|pushnotification|i-9|デバイスへのプッシュ通知の送信|
|remoteLock|個|デバイスをリモートでロックする|




