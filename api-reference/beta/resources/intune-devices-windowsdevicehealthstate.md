---
title: windowsdevicehealthstate 列挙型
description: コンピューターエンドポイントの保護の状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156169"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsdevicehealthstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンピューターエンドポイントの保護の状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|クリーン|.0|コンピューターがクリーンであり、アクションは必要ありません|
|fullscanpending|1-d|コンピューターが保留中の完全なスキャン状態である|
|rebootPending|pbm-2|コンピューターが再起動の保留状態になっている|
|manualstepspending|2/4|コンピューターが保留中の手動の手順状態である|
|offlineScanPending|~|コンピューターが保留中のオフラインスキャン状態になっている|
|critical|16|コンピューターは重大なエラー状態です|




