---
title: androidRequiredPasswordType 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0562d059ca69358190c49fb6b518abccdc98c449
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028708"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 列挙型

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



