---
title: androiddeviceownerrequiredpasswordtype 列挙型
description: Android デバイスの所有者ポリシーに必要なパスワードの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c575b1b39592eb8191e358563abb6d6bd834e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556380"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androiddeviceownerrequiredpasswordtype 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイスの所有者ポリシーに必要なパスワードの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|デバイスの既定値。意図的ではありません。|
|必須|1 |パスワードを設定する必要がありますが、種類に制限はありません。|
|数値|2 |少なくとも数値。|
|numericcomplex|3 |繰り返しまたは順序付けられていない、少なくとも数値。|
|読み|4 |少なくとも英字のパスワード。|
|文字|5 |少なくとも英数字のパスワード|
|alphanumericWithSymbols|6 |記号を含む、少なくとも英数字。|
|lowsecuritybiometric 認証|7 |低セキュリティ生体認証ベースのパスワードが必要です。|





