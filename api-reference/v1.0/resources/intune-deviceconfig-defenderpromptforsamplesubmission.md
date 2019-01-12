---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e103916bd55e6c2d505a85c379b80962ab9a0cac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928088"
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



