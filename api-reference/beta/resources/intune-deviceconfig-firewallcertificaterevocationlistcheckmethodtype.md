---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbfad062f551bbf53c0e0e27fe40611d6f70dd0e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985866"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

FirewallCertificateRevocationListCheckMethod に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|.0|Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない|
|none|1-d|証明書失効リストをチェックしない|
|再試行|pbm-2|証明書がチェックで確認されている場合にのみ、CRL の確認と許可を試行します。|
|要する|1/3|証明書を許可する前に、正常な CRL チェックを必要とする|





