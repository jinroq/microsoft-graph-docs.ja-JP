---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548461"
---
# <a name="actionstate-enum-type"></a>actionstate 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス上のアクションの状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|なし|.0|有効なアクション状態ではありません|
|対する|1 |アクションが保留中|
|取り消す|2 |アクションが取り消されました。|
|active|3 |アクションはアクティブです。|
|done|4 |操作はエラーなしで完了しました。|
|フェール|5 |アクションの失敗|
|notSupported|6 |アクションはサポートされていません。|



