---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: firewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e3a74122f0b0a9fe1a6dfab40593123ec8709c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160817"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>firewallPreSharedKeyEncodingMethodType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

firewallPreSharedKeyEncodingMethod に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない|
|none|1-d|事前共有キーはエンコードされていません。 代わりに、ワイド文字形式で保存されます。|
|utF8|pbm-2|utf-8 を使用して事前共有キーをエンコードする|




