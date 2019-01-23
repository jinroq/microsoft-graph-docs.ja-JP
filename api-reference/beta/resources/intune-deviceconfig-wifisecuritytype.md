---
title: wiFiSecurityType 列挙型
description: Wi-fi セキュリティの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422132"
---
# <a name="wifisecuritytype-enum-type"></a>wiFiSecurityType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




