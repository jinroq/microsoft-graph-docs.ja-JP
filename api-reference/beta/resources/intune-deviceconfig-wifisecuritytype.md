---
title: wiFiSecurityType 列挙型
description: Wi-fi セキュリティの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85c317706bb953fdeef202e4df9ec114944a7630
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944440"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Wi-fi セキュリティの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|開か|.0|開く (認証なし)。|
|wpaPersonal|1-d|WPA-個人用。|
|wpaEnterprise|pbm-2|WPA-エンタープライズ。 エンタープライズオプションを構成するには、IOSEnterpriseWifiConfiguration type を使用する必要があります。|
|wep|1/3|WEP 暗号化。|
|wpa2Personal|2/4|WPA2-個人用。|
|wpa2Enterprise|5|WPA2-エンタープライズ。 エンタープライズオプションを構成するには、WindowsWifiEnterpriseEAPConfiguration type を使用する必要があります。|




