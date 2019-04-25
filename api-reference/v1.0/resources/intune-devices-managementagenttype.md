---
title: managementagenttype 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522714"
---
# <a name="managementagenttype-enum-type"></a>managementagenttype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理エージェントの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|eas|1 |デバイスは、Exchange server によって管理されています。|
|mdm.exe|2 |デバイスは Intune MDM によって管理されます。|
|easmdm|3 |デバイスは、Exchange server と Intune MDM の両方によって管理されます。|
|intアンの場合|4 |Intune クライアント管理。|
|easintアンの場合|5 |デバイスは EAS で、Intune クライアントはデュアル管理されています。|
|configurationmanagerclient|8 |デバイスは構成マネージャーによって管理されています。|
|configurationmanagerclientmdm|10  |デバイスは、構成マネージャーおよび MDM によって管理されます。|
|configurationmanagerclientmdmeas|11 |デバイスは、構成マネージャー、MDM、Eas によって管理されます。|
|不明|16 |管理エージェントの種類が不明です。|
|jamf|32|デバイス属性は、Jamf から取得されます。|
|googleCloudDevicePolicyController|64|デバイスは Google の CloudDPC によって管理されています。|



