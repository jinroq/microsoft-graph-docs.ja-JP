---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4585c30c0a910befd8df8482636916af9ad9c0d6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396414"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

FirewallCertificateRevocationListCheckMethod に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合|
|none|1|証明書失効リストをチェックしません。|
|試行|2|CRL チェックを試みるし、チェックして、証明書が確認される場合にのみ証明書を許可します。|
|必要|3|証明書を許可する前に成功した CRL チェックが必要|




