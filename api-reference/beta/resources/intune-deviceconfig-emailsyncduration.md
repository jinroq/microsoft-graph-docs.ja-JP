---
title: emailSyncDuration 列挙型
description: 電子メールに使用できる値は、時間を同期します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d83a1ceb82820ddc44d8753e8ed05e00de09e36e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819384"
---
# <a name="emailsyncduration-enum-type"></a>emailSyncDuration 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

電子メールに使用できる値は、時間を同期します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|直後|1|1 日分の電子メールを同期します。|
|3 日|2|3 日間の電子メールを同期します。|
|1 週間|3|1 週間分のメールを同期します。|
|2 週間|4|2 週間分のメールを同期します。|
|oneMonth|5|電子メールの 1 か月を同期します。|
|無制限|6|電子メールの無制限の時間を同期します。|





