---
title: androidForWorkRequiredPasswordType 列挙型
description: Android の作業には、パスワード入力が必要です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b7d64ce762b3c07af74e02ed0aa37accf615ef7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850212"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a>androidForWorkRequiredPasswordType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android の作業には、パスワード入力が必要です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|デバイスの既定値でことを目的しません。|
|lowSecurityBiometric|1|低レベルのセキュリティ ベースの生体認証パスワードが必要です。|
|必須|2|必須。|
|atLeastNumeric|3|数値以上のパスワードが必要です。|
|numericComplex|4|数値の複雑なパスワードが必要です。|
|atLeastAlphabetic|5|少なくともアルファベットのパスワードが必要です。|
|atLeastAlphanumeric|6|以上の英数字のパスワードが必要です。|
|alphanumericWithSymbols|7|少なくとも文字の英数字の記号のパスワードが必要です。|





