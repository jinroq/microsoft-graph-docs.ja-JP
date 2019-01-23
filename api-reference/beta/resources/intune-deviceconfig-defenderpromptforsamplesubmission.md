---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b706c0086791543a5cbb13d26ae1d86a2e3b1760
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403316"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

サンプル提出用のユーザーにメッセージを表示可能な値です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|alwaysPrompt|1|常にメッセージを表示します。|
|promptBeforeSendingPersonalData|2|個人データを送信する前にメッセージを表示します。|
|neverSendData|3|データを送信しないでください。|
|sendAllDataWithoutPrompting|4|メッセージを表示せず、すべてのデータを送信します。|




