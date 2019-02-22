---
title: wiFiSecurityType 列挙型
description: wi-fi セキュリティの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c16265ecf9b4fa56536838dde1f4f1f757d8b1f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159046"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

wi-fi セキュリティの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|開か|.0|開く (認証なし)。|
|wpaPersonal|1-d|WPA-個人用。|
|wpaenterprise|pbm-2|WPA-エンタープライズ。 エンタープライズオプションを構成するには、IOSEnterpriseWifiConfiguration type を使用する必要があります。|
|wep|1/3|WEP 暗号化。|
|wpa2Personal|2/4|WPA2-個人用。|
|wpa2Enterprise|5|WPA2-エンタープライズ。 エンタープライズオプションを構成するには、WindowsWifiEnterpriseEAPConfiguration type を使用する必要があります。|




