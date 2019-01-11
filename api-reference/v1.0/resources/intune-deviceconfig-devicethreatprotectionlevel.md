---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa287d9259ed88f1b2240fd9bbdcaf77bcf9170e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850583"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスの脅威保護 API のデバイスの脅威保護レベルです。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|利用不可|0|既定値です。 使用しないでください。|
|セキュリティで保護|1|デバイスの脅威のレベルの要件: セキュリティで保護します。 これは、最も安全なレベルであり、デバイス上の脅威が見つかりませんだったことを表します。|
|低|2|デバイスの脅威保護に必要なレベル: 低。 低は、デバイスまたはデバイスのデータに最小限のリスクをもたらす脅威の重大度レベルを表します。|
|medium|3|デバイスの脅威保護に必要なレベル: 中。 [中] では、中程度のデバイスまたはデバイスのデータへのリスクをポーズする脅威の重大度レベルを表します。|
|高|4|デバイスの脅威保護に必要なレベル: 高。 高では、デバイスまたはデバイスのデータに重大なリスクをもたらす脅威の重大度レベルを表します。|
|notSet|10|デバイスの脅威保護に必要なレベル: 設定されていません。 セットはない、脅威保護のレベルを満たすためにデバイスの要件がないことです。|



