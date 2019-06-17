---
title: androidRequiredPasswordType 列挙型
description: Android 必要なパスワードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2cfbf31bc2c263031e2e850e4caf479abb325ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988951"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android 必要なパスワードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|.0|デバイスの既定値。意図的ではありません。|
|読み|1-d|アルファベットのパスワードが必要です。|
|文字|pbm-2|英数字のパスワードが必要です。|
|alphanumericWithSymbols|1/3|記号パスワードが必要な英数字。|
|lowSecurityBiometric 認証|2/4|低セキュリティ生体認証ベースのパスワードが必要です。|
|数値|5|数字のパスワードが必要です。|
|numericComplex|シックス|数字の複雑なパスワードが必要です。|
|any|7|パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。|





