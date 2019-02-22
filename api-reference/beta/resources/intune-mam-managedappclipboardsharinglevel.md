---
title: managedappクリップボード sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 352a801c53acd487fdac0206eca828461d35bf68
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148350"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedappクリップボード sharinglevel 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーション間でデバイスのクリップボードを共有するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|allapps|.0|すべてのアプリ間での共有が可能、管理されている|
|managedAppsWithPasteIn|1-d|[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。|
|managedApps|pbm-2|すべての管理対象アプリ間で共有が可能|
|ブロック|1/3|アプリ間の共有が無効になっている|




