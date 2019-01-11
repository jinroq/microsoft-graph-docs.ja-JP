---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 06a89256920f143af923e6a3949e61843fa7aa00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814421"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android では、パスワード入力が必要です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|デバイスの既定値でことを目的しません。|
|アルファベット|1|アルファベットのパスワードが必要です。|
|英数字|2|英数字のパスワードが必要です。|
|alphanumericWithSymbols|3|文字の英数字の記号のパスワードが必要です。|
|lowSecurityBiometric|4|低レベルのセキュリティ ベースの生体認証パスワードが必要です。|
|numeric|5|数字のパスワードが必要です。|
|numericComplex|6|数値の複雑なパスワードが必要です。|
|any|7|パスワードまたはパターンは、必須では、いずれかの許容可能です。|



