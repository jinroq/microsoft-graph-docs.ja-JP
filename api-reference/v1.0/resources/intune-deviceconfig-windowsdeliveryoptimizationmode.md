---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021599"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

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



