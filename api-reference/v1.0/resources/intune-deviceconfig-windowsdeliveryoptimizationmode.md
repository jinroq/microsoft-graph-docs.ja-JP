---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f80c6b5cbe7316c851954154bdb559f370f02b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951517"
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



