---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
ms.openlocfilehash: df51851ef0820f5982a6689421503364e9064c78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069238"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>vpnTrafficRuleRoutingPolicyType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

VPN トラフィックの規則のルーティング ポリシーを指定します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|ルーティング ポリシーが指定されていません。|
|splitTunnel|1|指定したアプリケーションのネットワーク トラフィックは、VPN を介してルーティングされます。|
|forceTunnel|2|すべてのネットワーク トラフィックは、VPN を介してルーティングされます。|





