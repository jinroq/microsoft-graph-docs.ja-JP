---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd370f9e706955d76de519a518b4659ba46c6d25
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250916"
---
# <a name="devicecomplianceactiontype-enum-type"></a>devicecomplianceactiontype 列挙型

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



