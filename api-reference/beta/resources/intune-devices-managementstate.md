---
title: managementState 列挙型
description: Microsoft Intune でのデバイスの状態を管理します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c439cf0ff830f471d2050eee81c91c6539e66d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844654"
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





