---
title: androidforwork requiredpasswordtype 列挙型
description: Android 用 Android が必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bfdca6204bd1745fc9a8350309e51cec2a8a718
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775724"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a>androidforwork requiredpasswordtype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android 用 Android が必要なパスワードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|デバイスの既定値。意図的ではありません。|
|lowsecuritybiometric 認証|1-d|低セキュリティ生体認証ベースのパスワードが必要です。|
|必須|pbm-2|必須。|
|atleastnumeric|1/3|少なくとも数値のパスワードが必要です。|
|numericcomplex|2/4|数字の複雑なパスワードが必要です。|
|atall stアルファベット|5|少なくとも英字のパスワードが必要です。|
|atleastalphanumeric|シックス|少なくとも英数字のパスワードが必要です。|
|alphanumericWithSymbols|7|記号パスワードが必要な、少なくとも英数字。|





