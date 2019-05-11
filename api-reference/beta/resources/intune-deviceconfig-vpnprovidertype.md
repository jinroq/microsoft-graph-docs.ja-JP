---
title: vpnProviderType 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df2fffa2c18ff21f342b2de0fdd8d7cd0d60ca64
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944552"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリごとの VPN のプロバイダーの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|トンネルトラフィックは明示的に構成されていません。|
|appProxy|1-d|アプリケーション層でのトンネルトラフィック。|
|packetTunnel|pbm-2|IP 層でのトンネルトラフィック。|




