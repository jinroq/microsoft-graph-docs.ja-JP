---
title: windowsDeliveryOptimizationMode 列挙型
description: ピア配布の配信最適化モード
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554150"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ピア配布の配信最適化モード

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|httpOnly|1 |HTTP のみ、ピアリングなし|
|httpWithPeeringNat|2 |OS 既定–同一ネットワークアドレス変換の背後でピアリングを使用して Http を融合したもの|
|httpWithPeeringPrivateGroup|3 |プライベートグループ間でのピアリングとの HTTP ブレンディング|
|httpwithinternetpeering リング|4 |インターネットピアリングとの HTTP ブレンディング|
|simpledownload|99|ピアリングのない簡易ダウンロードモード|
|bypassMode|100|バイパスモード。 配信の最適化を使用せず、代わりにビットを使用する|





