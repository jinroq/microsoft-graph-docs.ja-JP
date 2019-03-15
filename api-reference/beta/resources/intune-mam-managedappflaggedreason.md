---
title: managedappflaggedreason 列挙型
description: ユーザーにフラグが設定された理由
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15942be9f9b6d8b25941f0726ff6046feeea386b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572160"
---
# <a name="managedappflaggedreason-enum-type"></a>managedappflaggedreason 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーにフラグが設定された理由

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|なし|.0|問題はありません。|
|rootedDevice|1|アプリの登録は、ルート/ロック解除されたデバイス上で実行されています。|
|androidBootloaderUnlocked|2|アプリの登録は、ブートローダーのロックが解除されている Android デバイス上で実行されています。|
|androidFactoryRomModified|1/3|アプリの登録は、工場 ROM が変更された Android デバイス上で実行されています。|




