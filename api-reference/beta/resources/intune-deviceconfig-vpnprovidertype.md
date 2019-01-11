---
title: vpnProviderType 列挙型
description: アプリケーションごとの vpn プロバイダーの種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea3e3fcac5fc84270fcdb63b6ab673cb9f55aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861286"
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





