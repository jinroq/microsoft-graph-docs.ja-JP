---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者のポリシーでは、パスワード入力が必要です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403540"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイスの所有者のポリシーでは、パスワード入力が必要です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|デバイスの既定値でことを目的しません。|
|必須|1|パスワードのセットでは、必要がありますが、型に制限はありません。|
|numeric|2|At は最低の数値です。|
|numericComplex|3|At なしまたは繰り返しの順序付けられたシーケンスでは、少なくとも数値です。|
|アルファベット|4|少なくともアルファベットのパスワードです。|
|英数字|5|以上の英数字のパスワード|
|alphanumericWithSymbols|6|少なくとも文字の英数字の記号です。|




