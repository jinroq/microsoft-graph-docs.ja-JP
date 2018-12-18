---
title: wiFiSecurityType 列挙型
description: Wi-fi セキュリティの種類です。
author: tfitzmac
ms.openlocfilehash: 291bc3660971a90ea113959368542e715a86b570
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329191"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Wi-fi セキュリティの種類です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|開く|0|(認証なし) を開きます。|
|wpaPersonal|1|WPA-パーソナルです。|
|wpaEnterprise|2|WPA-エンタープライズ。 エンタープライズ オプションを構成するのには IOSEnterpriseWifiConfiguration 型を使用する必要があります。|
|wep|3|WEP 暗号化します。|
|wpa2Personal|4|WPA2-パーソナルです。|
|wpa2Enterprise|5|WPA2-エンタープライズ。 エンタープライズ オプションを構成するのには WindowsWifiEnterpriseEAPConfiguration 型を使用する必要があります。|





