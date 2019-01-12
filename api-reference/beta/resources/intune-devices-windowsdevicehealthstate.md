---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923944"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





