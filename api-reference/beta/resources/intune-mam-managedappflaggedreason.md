---
title: managedAppFlaggedReason 列挙型
description: ユーザーにフラグが設定された理由
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b07670130f386a5b4a3c53495464652aee7e686
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996289"
---
# <a name="managedappflaggedreason-enum-type"></a>managedAppFlaggedReason 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーにフラグが設定された理由

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|問題はありません。|
|rootedDevice|1-d|アプリの登録は、ルート/ロック解除されたデバイス上で実行されています。|
|androidBootloaderUnlocked|pbm-2|アプリの登録は、ブートローダーのロックが解除されている Android デバイス上で実行されています。|
|androidFactoryRomModified|1/3|アプリの登録は、工場 ROM が変更された Android デバイス上で実行されています。|





