---
title: actionState 列挙型
description: デバイス上のアクションの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35fccdc65eec7781f38d366e31ddb1a626005169
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996226"
---
# <a name="actionstate-enum-type"></a>actionState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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





