---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a5b908b3d978c6a05897f466e43651b50f9931b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974984"
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



