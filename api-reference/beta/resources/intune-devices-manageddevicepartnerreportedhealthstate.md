---
title: manageddevicepartnerreportedhealthstate 列挙型
description: デバイス正常性 API の利用可能な状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60a3071094e2667b896401c6df29977f9923884c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143772"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>manageddevicepartnerreportedhealthstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|セキュリティ|~|脅威の防御パートナーによってデバイスが侵害されたと見なされます。 これは、デバイスのアクティブな脅威またはリスクが、エンドユーザーによって簡単に修復できず、ユーザーが IT 管理者に連絡する必要があることを意味します。|
|誤った|i-9|脅威の防御パートナーとの間でデバイスが正しく構成されていないと考えられます。 これは、脅威またはリスク分析が正常に機能するために必要なプロファイルまたは構成がデバイスにないことを意味します。そのため、脅威またはリスク分析を完了できません。|




