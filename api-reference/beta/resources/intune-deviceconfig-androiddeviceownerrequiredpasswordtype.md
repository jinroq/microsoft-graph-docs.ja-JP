---
title: androiddeviceownerrequiredpasswordtype 列挙型
description: Android デバイスの所有者ポリシーに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79d71fbabc4597c87c9cee782904334e2f12d7e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172591"
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
|numeric|pbm-2|少なくとも数値。|
|numericcomplex|1/3|繰り返しまたは順序付けられていない、少なくとも数値。|
|読み|2/4|少なくとも英字のパスワード。|
|英数字|5|少なくとも英数字のパスワード|
|alphanumericWithSymbols|シックス|記号を含む、少なくとも英数字。|




