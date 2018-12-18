---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
author: tfitzmac
ms.openlocfilehash: 5aa3f44f0e4ccf177154f97e9849093c52728b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343422"
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





