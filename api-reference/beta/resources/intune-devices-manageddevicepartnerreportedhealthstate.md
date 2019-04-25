---
title: manageddevicepartnerreportedhealthstate 列挙型
description: デバイス正常性 API の利用可能な状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04ed30c087bb9f607f1579819d09def103658ca3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521272"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>manageddevicepartnerreportedhealthstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス正常性 API の利用可能な状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|デバイス正常性状態はまだ報告されていません|
|アクティブ化|1 |デバイスは、モバイル脅威防衛パートナーによってアクティブ化されていますが、正常性を報告していません。|
|不可|2 |モバイル脅威防御パートナーによってデバイスが非アクティブ化されました。 デバイスの正常性が不明です。|
|セキュリティ保護|3 |モバイル脅威防御パートナーによって、デバイスはセキュリティで保護されていると見なされます。|
|lowSeverity|4 |モバイル脅威防御パートナーによって、デバイスの脅威は低いと見なされます。|
|mediumSeverity|5 |モバイル脅威防御パートナーによって、デバイスは中程度の脅威と見なされます。|
|highSeverity|6 |モバイル脅威防御パートナーによって、デバイスが高い脅威と見なされます。|
|なかっ|7 |モバイル脅威防御パートナーによってデバイスが応答しないと見なされます。 デバイスの正常性が不明です。|
|セキュリティ|8 |脅威の防御パートナーによってデバイスが侵害されたと見なされます。 これは、デバイスのアクティブな脅威またはリスクが、エンドユーザーによって簡単に修復できず、ユーザーが IT 管理者に連絡する必要があることを意味します。|
|誤った|9 |脅威の防御パートナーとの間でデバイスが正しく構成されていないと考えられます。 これは、脅威またはリスク分析が正常に機能するために必要なプロファイルまたは構成がデバイスにないことを意味します。そのため、脅威またはリスク分析を完了できません。|





