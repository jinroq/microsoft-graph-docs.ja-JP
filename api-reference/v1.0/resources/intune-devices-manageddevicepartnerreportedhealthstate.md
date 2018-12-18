---
title: managedDevicePartnerReportedHealthState 列挙型
description: デバイス状態の API の使用可能な状態
author: tfitzmac
ms.openlocfilehash: 56935f924c0796fe0db1be7b34a4782b5072784f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301079"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState 列挙型

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



