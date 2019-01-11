---
title: managedDevicePartnerReportedHealthState 列挙型
description: デバイス状態の API の使用可能な状態
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e3383edca25d6d4ac03a9b5536f3514412e2bf7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862056"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス状態の API の使用可能な状態
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|デバイスの正常性の状態はレポートされていません。|
|アクティブ化|1|デバイスは、モバイルの脅威の防御のパートナー様が済んでいるは、まだ状態を報告します。|
|非アクティブ化|2|モバイルの脅威の防御のパートナーでは、デバイスを無効化されています。 デバイスの状態が不明です。|
|セキュリティで保護|3|デバイスは、モバイルの脅威の防御のパートナーによってセキュリティで保護されたと見なされます。|
|lowSeverity|4|デバイスは、モバイルの脅威の防御のパートナーによって、低レベルの脅威と見なされます。|
|mediumSeverity|5|デバイスは、モバイルの脅威の防御のパートナーが中レベルの脅威と見なされます。|
|highSeverity|6|デバイスは、モバイルの脅威の防御のパートナーが高レベルの脅威と見なされます。|
|応答しません。|7|デバイスは、モバイルの脅威の防御のパートナーが応答しなくなったと見なされます。 デバイスの状態が不明です。|
|危険にさらされました。|8|デバイスでは、脅威に対する防御のパートナーが危険にさらされたと見なされます。 つまり、デバイスには、作業中の脅威やリスクをエンド ・ ユーザーによって容易に改善することはできませんし、ユーザーは、IT 管理者に連絡する必要があります。|
|構成が正しくありません。|9|デバイスでは、脅威に対する防御のパートナーで正しく構成されていないと見なされます。 つまりデバイスが必要なプロファイルまたは正常に機能する脅威の防御のパートナーの構成が存在しませんし、脅威は、このようにリスク分析が完了することはありません。|





