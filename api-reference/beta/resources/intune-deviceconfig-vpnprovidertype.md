---
title: vpnProviderType 列挙型
description: アプリケーションごとの vpn プロバイダーの種類。
author: tfitzmac
ms.openlocfilehash: d8f002582879302bcbe0fb965110eaa5e674a689
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351598"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリケーションごとの vpn プロバイダーの種類。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|トンネル トラフィックが明示的に構成されていません。|
|appProxy|1|アプリケーション レイヤーでトラフィックをトンネルします。|
|packetTunnel|2|IP 層でトラフィックをトンネリングします。|





