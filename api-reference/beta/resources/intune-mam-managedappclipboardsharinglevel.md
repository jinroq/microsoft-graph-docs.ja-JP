---
title: Managedappクリップボード Sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7c03aeffe8e83a51caadba952e09af1fce06593
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991983"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>Managedappクリップボード Sharinglevel 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーション間でデバイスのクリップボードを共有するレベルを表します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|allApps|.0|すべてのアプリ間での共有が可能、管理されている|
|managedAppsWithPasteIn|1-d|[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。|
|managedApps|pbm-2|すべての管理対象アプリ間で共有が可能|
|ブロック|1/3|アプリ間の共有が無効になっている|





