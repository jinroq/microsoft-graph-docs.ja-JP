---
title: defendercloudblockleveltype 列挙型
description: クラウドブロックレベルの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258836"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defendercloudblockleveltype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

クラウドブロックレベルの可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。|
|高額|1-d|High は、強力なレベルの検出を適用します。|
|highplus|pbm-2|高 + は高レベルを使用し、追加の保護対策を適用します。|
|zeroTolerance|1/3|ゼロトレランスによってすべての不明な実行可能ファイルがブロック|



