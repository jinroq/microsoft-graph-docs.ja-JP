---
title: defendercloudblockleveltype 列挙型
description: クラウドブロックレベルの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88872e6d37afd1820559018bff6943e3ee623a0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563533"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defendercloudblockleveltype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

クラウドブロックレベルの可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。|
|高額|1 |High は、強力なレベルの検出を適用します。|
|highplus|2 |高 + は高レベルを使用し、追加の保護対策を適用します。|
|zeroTolerance|3 |ゼロトレランスによってすべての不明な実行可能ファイルがブロック|





