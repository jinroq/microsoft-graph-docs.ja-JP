---
title: vpnProviderType 列挙型
description: アプリケーションごとの vpn プロバイダーの種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2de8f78222ba0c945000b84f28039c2f6af58daa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407222"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーションごとの vpn プロバイダーの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|トンネル トラフィックが明示的に構成されていません。|
|appProxy|1|アプリケーション レイヤーでトラフィックをトンネルします。|
|packetTunnel|2|IP 層でトラフィックをトンネリングします。|




