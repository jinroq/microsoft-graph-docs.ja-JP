---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
ms.openlocfilehash: 601531dd71ee0d44e9f5ebc89eb018ba5e0f2675
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066342"
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





