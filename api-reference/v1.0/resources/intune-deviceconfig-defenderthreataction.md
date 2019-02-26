---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252316"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

検出されたマルウェアの脅威を処理する Defender の既定のアクション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|更新定義に基づいてアクションを適用します。|
|クリーン|1-d|検出された脅威を除去します。|
|済み|pbm-2|検出された脅威を検疫します。|
|remove|1/3|検出された脅威を削除します。|
|使う|2/4|検出された脅威を許可します。|
|自分のもの|5|検出された脅威に対して実行するアクションをユーザーが決定できるようにします。|
|拒否|シックス|検出された脅威をブロックします。|



