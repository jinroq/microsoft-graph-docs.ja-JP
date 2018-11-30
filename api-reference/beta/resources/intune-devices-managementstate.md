---
title: managementState 列挙型
description: Microsoft Intune でのデバイスの状態を管理します。
ms.openlocfilehash: 554e06ff32102285d4851a19350c7c44d11d1fb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072551"
---
# <a name="managementstate-enum-type"></a>managementState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Microsoft Intune でのデバイスの状態を管理します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|管理|0|管理対象デバイスは、します。|
|retirePending|1|削除コマンドは、デバイスと管理から unenrolling の処理中に発生しています。|
|retireFailed|2|破棄コマンドがデバイスに失敗しました。|
|wipePending|3|ワイプ コマンドは、デバイスと管理から unenrolling の処理中に発生しています。|
|wipeFailed|4|デバイス ワイプ コマンドが失敗しました。|
|問題があります。|5|デバイスが正常な状態ではありません。|
|deletePending|6|削除コマンドは、デバイスで発生しています。 |
|retireIssued|7|デバイスの削除コマンドが発行されました|
|wipeIssued|8|デバイス ワイプ コマンドがに対して発行されました|
|wipeCanceled|9|このデバイスのワイプ コマンドがキャンセルされました|
|retireCanceled|10|このデバイスの削除コマンドがキャンセルされました|
|発見|11|デバイスが検出されたが、完全に登録されています。|





