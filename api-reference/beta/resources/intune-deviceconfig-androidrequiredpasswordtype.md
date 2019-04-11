---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782073"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidrequiredpasswordtype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android 必要なパスワードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|デバイスの既定値。意図的ではありません。|
|読み|1-d|アルファベットのパスワードが必要です。|
|文字|pbm-2|英数字のパスワードが必要です。|
|alphanumericWithSymbols|1/3|記号パスワードが必要な英数字。|
|lowsecuritybiometric 認証|2/4|低セキュリティ生体認証ベースのパスワードが必要です。|
|数値|5|数字のパスワードが必要です。|
|numericcomplex|シックス|数字の複雑なパスワードが必要です。|
|any|7|パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。|





