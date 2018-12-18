---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 255aab9770305baa29e73278b3bfceec1079351a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321001"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|不明な割り当ての状態|
|assignedInSync|1|Intune で正常に割り当てられていると Windows の自動パイロット プログラムとの同期|
|assignedOutOfSync|2|Intune で正常に割り当てられているといないと同期させる Windows 自動パイロット プログラム|
|assignedUnkownSyncState|3|Intune といずれかの同期で正常に割り当てられているまたは Windows 自動パイロット プログラムとの同期|
|notAssigned|4|割り当てられていません。|
|保留中|5|保留中の割り当て|
|失敗しました。|6| 割り当てに失敗しました。|





