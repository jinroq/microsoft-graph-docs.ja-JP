---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793463"
---
# <a name="actionstate-enum-type"></a>actionstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

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





