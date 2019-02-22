---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5d1af0e6c91dced1aa12ae72c22430d16674c21
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156379"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|不明な割り当て状態|
|assignedInSync|1-d|Intune で正常に割り当てられ、Windows 自動パイロットプログラムとの同期|
|assignedOutOfSync|pbm-2|Intune で正常に割り当てられ、Windows 自動パイロットプログラムと同期されません|
|assignedUnkownSyncState|1/3|Intune で正常に割り当てられ、Windows 自動パイロットプログラムとの間で同期されているか、同期されていません|
|notAssigned|2/4|未割り当て|
|対する|5|保留中の割り当て|
|フェール|シックス| 割り当て失敗|




