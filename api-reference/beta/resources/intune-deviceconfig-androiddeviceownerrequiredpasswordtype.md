---
title: androiddeviceownerrequiredpasswordtype 列挙型
description: Android デバイスの所有者ポリシーに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 376e33edac921f6771d76a45622a58bca3076c5c
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572335"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androiddeviceownerrequiredpasswordtype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイスの所有者ポリシーに必要なパスワードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|デバイスの既定値。意図的ではありません。|
|必須|1-d|パスワードを設定する必要がありますが、種類に制限はありません。|
|数値|pbm-2|少なくとも数値。|
|numericcomplex|1/3|繰り返しまたは順序付けられていない、少なくとも数値。|
|読み|2/4|少なくとも英字のパスワード。|
|文字|5|少なくとも英数字のパスワード|
|alphanumericWithSymbols|シックス|記号を含む、少なくとも英数字。|
|lowsecuritybiometric 認証|7|低セキュリティ生体認証ベースのパスワードが必要です。|




