---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
ms.openlocfilehash: e08df0ef61b6d60227f9dec2382a57884c2f4bdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355987"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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





