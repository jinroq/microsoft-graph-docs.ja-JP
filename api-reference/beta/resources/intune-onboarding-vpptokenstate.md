---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
ms.openlocfilehash: 7180364063a48e1b0eeb2778ed4def7c0d3930a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069713"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|既定の状態。|
|有効です|1|トークンは、有効です。|
|有効期限が切れてください。|2|トークンの期限が切れています。|
|無効です|3|トークンが有効ではありません。|
|assignedToExternalMDM|4|トークンは、別の MDM サービスによって管理されます。|





