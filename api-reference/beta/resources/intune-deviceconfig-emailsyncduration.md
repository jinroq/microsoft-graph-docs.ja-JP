---
title: emailSyncDuration 列挙型
description: 電子メールに使用できる値は、時間を同期します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcabbe69c10cd490732560ea856c39c5cfd8cb44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986412"
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





