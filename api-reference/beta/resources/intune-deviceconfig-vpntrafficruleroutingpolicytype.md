---
title: vpnTrafficRuleRoutingPolicyType 列挙型
description: VPN トラフィックルールのルーティングポリシーを指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cbbba22017a40ae2f7db41e25f497c09156a2f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969374"
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





