---
title: deviceThreatProtectionLevel 列挙型
description: デバイス脅威保護 API のデバイスの脅威保護レベル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bb951e262993b2aee16d911eca10d638f08847a1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332723"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス脅威保護 API のデバイスの脅威保護レベル。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|無効|.0|既定値です。 使用しないでください。|
|セキュリティ保護|1-d|デバイスの脅威レベルの要件: セキュリティで保護されています。 これは最も安全なレベルで、デバイス上に脅威が何も検出されなかったことを表します。|
|低さ|pbm-2|デバイスの脅威保護レベルの要件: 低。 Low は、デバイスまたはデバイスのデータに対するリスクを最小限に抑える脅威の重要度を表します。|
|medium|1/3|デバイスの脅威保護レベルの要件: 中。 Medium は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。|
|高額|2/4|デバイスの脅威保護レベルの要件: High。 High は、デバイスまたはデバイスデータに重大なリスクをもたらす脅威の重要度を表します。|
|notSet|10 |デバイスの脅威保護レベルの要件: 設定されていません。 Not set は、デバイスが脅威保護レベルを満たすための要件がないことを表します。|



