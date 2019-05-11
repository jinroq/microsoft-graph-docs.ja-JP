---
title: windowsDeviceHealthState 列挙型
description: コンピューターエンドポイントの保護の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6086dc05d204e4c9cb23c77f79f98c3a207de35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941892"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンピューターエンドポイントの保護の状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|汚れ|.0|コンピューターがクリーンであり、アクションは必要ありません|
|fullScanPending|1-d|コンピューターが保留中の完全なスキャン状態である|
|rebootPending|pbm-2|コンピューターが再起動の保留状態になっている|
|manualStepsPending|2/4|コンピューターが保留中の手動の手順状態である|
|offlineScanPending|8 |コンピューターが保留中のオフラインスキャン状態になっている|
|critical|16|コンピューターは重大なエラー状態です|




