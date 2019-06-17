---
title: vpnProviderType 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23d8382c535a459beaf22d8cf229d0f6b3a50237
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987552"
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





