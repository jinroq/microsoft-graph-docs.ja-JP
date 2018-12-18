---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
author: tfitzmac
ms.openlocfilehash: 36a9790b669c588205824be60d350d2750637b15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312748"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

サンプル提出用のユーザーにメッセージを表示可能な値です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|alwaysPrompt|1|常にメッセージを表示します。|
|promptBeforeSendingPersonalData|2|個人データを送信する前にメッセージを表示します。|
|neverSendData|3|データを送信しないでください。|
|sendAllDataWithoutPrompting|4|メッセージを表示せず、すべてのデータを送信します。|



