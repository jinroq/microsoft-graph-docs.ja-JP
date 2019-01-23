---
title: managementAgentType 列挙型
description: 管理エージェントの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401006"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理エージェントの種類です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ea|1|デバイスは、Exchange サーバーによって管理されます。|
|mdm|2|Intune MDM. で、デバイスを管理します。|
|easMdm|3|Intune MDM. と Exchange サーバーの両方がデバイス管理します。|
|intuneClient|4|Intune クライアントが管理されています。|
|easIntuneClient|5|デバイスは、EA と Intune クライアント デュアル管理です。|
|configurationManagerClient|8|デバイスは、構成マネージャーによって管理されます。|
|configurationManagerClientMdm|10|デバイスの管理は、構成マネージャーと MDM.|
|configurationManagerClientMdmEas|11|デバイスは、MDM および Ea は、構成マネージャーによって管理されます。|
|不明|16|不明な管理エージェントの種類です。|
|jamf|32|デバイス属性は、Jamf からフェッチされます。|
|googleCloudDevicePolicyController|64|デバイスは、Google の CloudDPC によって管理されます。|
|microsoft365ManagedMdm|258|Intune によって Microsoft 365 では、このデバイスが管理されます。|




