---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c85466cf722848efa684fc7b5643293d49de2459
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964089"
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



