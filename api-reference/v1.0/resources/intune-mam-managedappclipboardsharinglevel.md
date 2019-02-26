---
title: managedappクリップボード sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250027"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedappクリップボード sharinglevel 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーション間でデバイスのクリップボードを共有するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|allapps|.0|すべてのアプリ間での共有が可能、管理されている|
|managedAppsWithPasteIn|1-d|[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。|
|managedApps|pbm-2|すべての管理対象アプリ間で共有が可能|
|ブロック|1/3|アプリ間の共有が無効になっている|



