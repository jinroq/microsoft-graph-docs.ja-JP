---
title: managementAgentType 列挙型
description: 管理エージェントの種類です。
author: tfitzmac
ms.openlocfilehash: 702f71f3984bda34e31d0a614e45e387f45b587e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321589"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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





