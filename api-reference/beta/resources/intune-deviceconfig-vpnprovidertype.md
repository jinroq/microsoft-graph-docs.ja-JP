---
title: vpnprovidertype 列挙型
description: アプリごとの VPN のプロバイダーの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e47f4d20cb843b62928c6c66e468d00f5a4f743
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795997"
---
# <a name="vpnprovidertype-enum-type"></a>vpnprovidertype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリごとの VPN のプロバイダーの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|トンネルトラフィックは明示的に構成されていません。|
|appproxy|1-d|アプリケーション層でのトンネルトラフィック。|
|packettunnel|pbm-2|IP 層でのトンネルトラフィック。|





