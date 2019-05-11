---
title: androidDeviceOwnerWiFiSecurityType 列挙型
description: Android デバイス所有者の Wi-fi セキュリティの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b015aa8c2e56df0a919b580d09f1a1d7e8bbe0c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948990"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a>androidDeviceOwnerWiFiSecurityType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者の Wi-fi セキュリティの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|開か|.0|開く (認証なし)。|
|wep|1-d|WEP 暗号化。|
|wpaPersonal|pbm-2|WPA-Personal/WPA2-個人用。|
|wpaEnterprise|2/4|WPA-エンタープライズ/WPA2-エンタープライズ。 エンタープライズオプションを構成するには、AndroidDeviceOwnerEnterpriseWifiConfiguration type を使用する必要があります。|




