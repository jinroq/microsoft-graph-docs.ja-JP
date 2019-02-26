---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eb469516dd4ae960ae351843df31f07ead90edf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146341"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーにサンプル送信のプロンプトを表示するために使用できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|always プロンプト|1-d|常にプロンプトを表示します。|
|promptBeforeSendingPersonalData|pbm-2|個人データを送信する前にメッセージを表示します。|
|neverSendData|1/3|データを送信しません。|
|sendalldataメッセージを表示しない|2/4|メッセージを表示せずにすべてのデータを送信します。|




