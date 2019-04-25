---
title: androidrequiredpasswordtype 列挙型
description: Android 必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575171"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidrequiredpasswordtype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android 必要なパスワードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|デバイスの既定値。意図的ではありません。|
|読み|1 |アルファベットのパスワードが必要です。|
|文字|2 |英数字のパスワードが必要です。|
|alphanumericWithSymbols|3 |記号パスワードが必要な英数字。|
|lowsecuritybiometric 認証|4 |低セキュリティ生体認証ベースのパスワードが必要です。|
|数値|5 |数字のパスワードが必要です。|
|numericcomplex|6 |数字の複雑なパスワードが必要です。|
|any|7 |パスワードまたはパターンが必要であり、任意のものが受け入れ可能である。|



