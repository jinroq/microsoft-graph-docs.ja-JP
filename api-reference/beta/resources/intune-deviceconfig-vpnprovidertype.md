---
title: vpnProviderType 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 43e9c146fc30e9dfaadef45b42e45dcf0787f13f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969465"
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





