---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d55ff0419c6178668bbee921c149c8bc797ebff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143401"
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




