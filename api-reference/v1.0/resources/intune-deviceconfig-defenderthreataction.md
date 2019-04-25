---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534319"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

検出されたマルウェアの脅威を処理する Defender の既定のアクション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|更新定義に基づいてアクションを適用します。|
|汚れ|1 |検出された脅威を除去します。|
|済み|2 |検出された脅威を検疫します。|
|remove|3 |検出された脅威を削除します。|
|使う|4 |検出された脅威を許可します。|
|自分のもの|5 |検出された脅威に対して実行するアクションをユーザーが決定できるようにします。|
|拒否|6 |検出された脅威をブロックします。|



