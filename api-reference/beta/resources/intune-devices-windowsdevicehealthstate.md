---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
author: tfitzmac
ms.openlocfilehash: b794f8121132e396459f9198c644084690fe95b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326328"
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





