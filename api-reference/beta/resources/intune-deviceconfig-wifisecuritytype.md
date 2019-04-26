---
title: wiFiSecurityType 列挙型
description: wi-fi セキュリティの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9144a5761691b0a50e40370b1f4d2d08967f2c28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554843"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

wi-fi セキュリティの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|開か|.0|開く (認証なし)。|
|wpaPersonal|1 |WPA-個人用。|
|wpaenterprise|2 |WPA-エンタープライズ。 エンタープライズオプションを構成するには、IOSEnterpriseWifiConfiguration type を使用する必要があります。|
|wep|3 |WEP 暗号化。|
|wpa2Personal|4 |WPA2-個人用。|
|wpa2Enterprise|5 |WPA2-エンタープライズ。 エンタープライズオプションを構成するには、WindowsWifiEnterpriseEAPConfiguration type を使用する必要があります。|





