---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1c146b42eab11dab4d90de9b3b134fdd29327323
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969073"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ピア配布の配信最適化モード

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|httpOnly|1-d|HTTP のみ、ピアリングなし|
|httpWithPeeringNat|pbm-2|OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの|
|httpWithPeeringPrivateGroup|1/3|プライベートグループ間でのピアリングとの HTTP ブレンディング|
|httpWithInternetPeering リング|2/4|インターネットピアリングとの HTTP ブレンディング|
|simpleDownload|99|ピアリングのない簡易ダウンロードモード|
|bypassMode|100|バイパスモード。 配信の最適化を使用せず、代わりにビットを使用する|





