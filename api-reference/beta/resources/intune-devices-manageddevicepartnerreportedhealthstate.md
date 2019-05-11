---
title: managedDevicePartnerReportedHealthState 列挙型
description: デバイス正常性 API の利用可能な状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 751edd41692b12e6ed300b56ad03fd0271edc9d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941955"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス正常性 API の利用可能な状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|デバイス正常性状態はまだ報告されていません|
|アクティブ化|1-d|デバイスは、モバイル脅威防衛パートナーによってアクティブ化されていますが、正常性を報告していません。|
|不可|pbm-2|モバイル脅威防御パートナーによってデバイスが非アクティブ化されました。 デバイスの正常性が不明です。|
|セキュリティ保護|1/3|モバイル脅威防御パートナーによって、デバイスはセキュリティで保護されていると見なされます。|
|lowSeverity|2/4|モバイル脅威防御パートナーによって、デバイスの脅威は低いと見なされます。|
|mediumSeverity|5|モバイル脅威防御パートナーによって、デバイスは中程度の脅威と見なされます。|
|highSeverity|シックス|モバイル脅威防御パートナーによって、デバイスが高い脅威と見なされます。|
|なかっ|7|モバイル脅威防御パートナーによってデバイスが応答しないと見なされます。 デバイスの正常性が不明です。|
|セキュリティ|8 |脅威の防御パートナーによってデバイスが侵害されたと見なされます。 これは、デバイスのアクティブな脅威またはリスクが、エンドユーザーによって簡単に修復できず、ユーザーが IT 管理者に連絡する必要があることを意味します。|
|誤った|9 |脅威の防御パートナーとの間でデバイスが正しく構成されていないと考えられます。 これは、脅威またはリスク分析が正常に機能するために必要なプロファイルまたは構成がデバイスにないことを意味します。そのため、脅威またはリスク分析を完了できません。|




