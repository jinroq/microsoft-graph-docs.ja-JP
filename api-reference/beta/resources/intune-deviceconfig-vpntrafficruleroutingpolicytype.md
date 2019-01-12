---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックの規則のルーティング ポリシーを指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c8ec4303dc16c7cb0606e4b9cf86594446f571e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974953"
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





