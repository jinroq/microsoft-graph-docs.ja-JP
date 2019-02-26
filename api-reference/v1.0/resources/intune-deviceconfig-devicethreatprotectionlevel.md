---
title: deviceThreatProtectionLevel 列挙型
description: デバイス脅威保護 API のデバイスの脅威保護レベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af0231e15cfa815d3fd2e154adf180f3e0c0c43
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253296"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 列挙型

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



