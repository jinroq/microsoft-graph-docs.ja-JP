---
title: androidRequiredPasswordType 列挙型
description: Android では、パスワード入力が必要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eebc6b0ad6eed346927fd48a2dc1f82b5e529b28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392914"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>androidRequiredPasswordType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




