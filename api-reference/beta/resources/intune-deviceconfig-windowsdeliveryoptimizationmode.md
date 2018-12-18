---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
ms.openlocfilehash: b23bdc80bd8b1fb151f9e138e1a1802140455c4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333482"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ピア配布の配信最適化モード
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|設定するユーザーを許可します。|
|httpOnly|1|ないピアリングのみ、HTTP|
|httpWithPeeringNat|2|OS の既定値は – Http が同じネットワーク アドレス変換器の背後にあるピアリングとブレンド|
|httpWithPeeringPrivateGroup|3|HTTP は、プライベート グループ全体でピアリングとブレンド|
|httpWithInternetPeering|4|HTTP はインターネットのピアリングとブレンド|
|simpleDownload|99|ピアリングのない単純なダウンロード モード|
|bypassMode|100|バイパス モードにします。 配信の最適化を使用せず、代わりにビットを使用|





