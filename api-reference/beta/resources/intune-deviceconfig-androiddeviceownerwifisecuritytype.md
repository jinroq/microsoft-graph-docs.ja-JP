---
title: androidDeviceOwnerWiFiSecurityType 列挙型
description: Android デバイス所有者の wi-fi セキュリティの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 725a786de238d8965507dc590cfd200fd91b13e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983751"
---
# <a name="androiddeviceownerwifisecuritytype-enum-type"></a>androidDeviceOwnerWiFiSecurityType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android デバイス所有者の wi-fi セキュリティの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|開か|.0|開く (認証なし)。|
|wep|1-d|WEP 暗号化。|
|wpaPersonal|pbm-2|WPA-Personal/WPA2-個人用。|
|wpaEnterprise|2/4|WPA-エンタープライズ/WPA2-エンタープライズ。 エンタープライズオプションを構成するには、AndroidDeviceOwnerEnterpriseWifiConfiguration type を使用する必要があります。|





