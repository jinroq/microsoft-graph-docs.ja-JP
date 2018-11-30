---
title: androidDeviceOwnerRequiredPasswordType 列挙型
description: Android デバイスの所有者のポリシーでは、パスワード入力が必要です。
ms.openlocfilehash: 16f4bc59f2b4fa9f37989d1bc1978cdfacb2892c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070887"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





