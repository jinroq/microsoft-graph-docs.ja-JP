---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fb72b606633356fc2de5cc0c41862a49517b416
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963395"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>vpnTrafficRuleRoutingPolicyType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

VPN トラフィックルールのルーティングポリシーを指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|ルーティングポリシーが指定されていません。|
|splitTunnel|1-d|指定したアプリのネットワークトラフィックは、VPN 経由でルーティングされます。|
|forceTunnel|pbm-2|すべてのネットワークトラフィックは、VPN 経由でルーティングされます。|





