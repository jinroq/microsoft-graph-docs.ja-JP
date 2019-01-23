---
title: deviceThreatProtectionLevel 列挙型
description: デバイスの脅威保護 API のデバイスの脅威保護レベルです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411233"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




