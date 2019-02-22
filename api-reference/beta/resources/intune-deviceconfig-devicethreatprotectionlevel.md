---
title: deviceThreatProtectionLevel 列挙型
description: デバイス脅威保護 API のデバイスの脅威保護レベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ecdf54051b1545b842cbc3c49359b9a77f12e2e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140244"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス脅威保護 API のデバイスの脅威保護レベル。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|無効|.0|既定値です。 使用しないでください。|
|セキュリティ保護|1-d|デバイスの脅威レベルの要件: セキュリティで保護されています。 これは最も安全なレベルで、デバイス上に脅威が何も検出されなかったことを表します。|
|低さ|pbm-2|デバイスの脅威保護レベルの要件: 低。 Low は、デバイスまたはデバイスのデータに対するリスクを最小限に抑える脅威の重要度を表します。|
|medium|1/3|デバイスの脅威保護レベルの要件: 中。 Medium は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。|
|高額|2/4|デバイスの脅威保護レベルの要件: High。 High は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。|
|notSet|個|デバイスの脅威保護レベルの要件: 設定されていません。 Not set は、デバイスが脅威保護レベルを満たすための要件がないことを表します。|




