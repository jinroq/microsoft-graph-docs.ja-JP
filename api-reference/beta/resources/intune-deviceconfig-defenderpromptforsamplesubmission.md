---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c81fe62d7ed2696b233b8684c665f7cf8341fbcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534781"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーにサンプル送信のプロンプトを表示するために使用できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|always プロンプト|1 |常にプロンプトを表示します。|
|promptBeforeSendingPersonalData|2 |個人データを送信する前にメッセージを表示します。|
|neverSendData|3 |データを送信しません。|
|sendalldataメッセージを表示しない|4 |メッセージを表示せずにすべてのデータを送信します。|





