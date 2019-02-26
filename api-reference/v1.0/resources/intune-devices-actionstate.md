---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261489"
---
# <a name="actionstate-enum-type"></a>actionstate 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス上のアクションの状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|有効なアクション状態ではありません|
|対する|1-d|アクションが保留中|
|取り消す|pbm-2|アクションが取り消されました。|
|active|1/3|アクションはアクティブです。|
|done|2/4|操作はエラーなしで完了しました。|
|フェール|5|アクションの失敗|
|notSupported|シックス|アクションはサポートされていません。|



