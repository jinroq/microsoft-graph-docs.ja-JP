---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: firewallCertificateRevocationListCheckMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 789ba503887a7200491f3fdc307ccaeb302b3f05
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776788"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

firewallCertificateRevocationListCheckMethod に指定できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|devicedefault|.0|Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない|
|none|1-d|証明書失効リストをチェックしない|
|再試行|pbm-2|証明書がチェックで確認されている場合にのみ、CRL の確認と許可を試行します。|
|要する|1/3|証明書を許可する前に、正常な CRL チェックを必要とする|





