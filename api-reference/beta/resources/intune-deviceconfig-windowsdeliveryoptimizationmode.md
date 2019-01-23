---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406886"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




