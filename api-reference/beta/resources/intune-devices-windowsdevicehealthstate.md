---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416350"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

コンピューター エンドポイントの保護の状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|クリーン|0|コンピューターがクリーンであり、操作する必要はありません。|
|fullScanPending|1|コンピューターで保留中の状態の完全なスキャンは、|
|rebootPending|2|コンピューターで保留中の再起動の状態には|
|manualStepsPending|4|コンピューターで保留中の手動の手順の状態は、|
|offlineScanPending|8|オフライン スキャンの状態を保留中のコンピューターが、します。|
|critical|16|コンピューターが、重大なエラー状態|




