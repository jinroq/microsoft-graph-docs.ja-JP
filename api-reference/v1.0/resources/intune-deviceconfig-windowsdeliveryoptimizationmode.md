---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463895"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ピア配布の配信最適化モード

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|httpOnly|1-d|HTTP のみ、ピアリングなし|
|httpWithPeeringNat|pbm-2|OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの|
|httpWithPeeringPrivateGroup|1/3|プライベートグループ間でのピアリングとの HTTP ブレンディング|
|httpwithinternetpeering リング|2/4|インターネットピアリングとの HTTP ブレンディング|
|simpledownload|99|ピアリングのない簡易ダウンロードモード|
|bypassMode|100|バイパスモード。 配信の最適化を使用せず、代わりにビットを使用する|



