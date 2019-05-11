---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0d699639d9af02b751ad701e4e6132bdc016911
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944503"
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




