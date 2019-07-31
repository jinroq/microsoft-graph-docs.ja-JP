---
title: managementAgentType 列挙型
description: 管理エージェントの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae96113e687d406f5c0342b3b71fd63ea6de9918
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999753"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理エージェントの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|eas|1-d|デバイスは、Exchange server によって管理されています。|
|mdm.exe|pbm-2|デバイスは Intune MDM によって管理されます。|
|easMdm|1/3|デバイスは、Exchange server と Intune MDM の両方によって管理されます。|
|Intアンの場合|2/4|Intune クライアント管理。|
|Easintアンの場合|5|デバイスは EAS で、Intune クライアントはデュアル管理されています。|
|configurationManagerClient|8 |デバイスは構成マネージャーによって管理されています。|
|configurationManagerClientMdm|10 |デバイスは、構成マネージャーおよび MDM によって管理されます。|
|configurationManagerClientMdmEas|#|デバイスは、構成マネージャー、MDM、Eas によって管理されます。|
|不明|16|管理エージェントの種類が不明です。|
|jamf|32|デバイス属性は、Jamf から取得されます。|
|googleCloudDevicePolicyController|64|デバイスは Google の CloudDPC によって管理されています。|
|microsoft365ManagedMdm|258|このデバイスは、Microsoft 365 によって Intune によって管理されます。|





