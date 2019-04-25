---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566032"
---
# <a name="devicecomplianceactiontype-enum-type"></a>devicecomplianceactiontype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

スケジュールされたアクションの種類列挙

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAction|.0|アクションなし|
|お知らせ|1 |通知の送信|
|拒否|2 |AAD でデバイスをブロックする|
|削除|3 |デバイスをインベントリから削除する|
|ふき|4 |デバイスをワイプする|
|removeresourceaccessprofiles|5 |デバイスからリソースアクセスプロファイルを削除する|
|pushnotification|9 |デバイスへのプッシュ通知の送信|
|remoteLock|10  |デバイスをリモートでロックする|





