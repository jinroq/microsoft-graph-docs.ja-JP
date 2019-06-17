---
title: windowsDeviceHealthState 列挙型
description: コンピューターエンドポイントの保護の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ac91095b27f7151d53ca81c43b3a77e3b8c0d87
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986593"
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





