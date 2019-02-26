---
title: managementagenttype 列挙型
description: 管理エージェントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251567"
---
# <a name="managementagenttype-enum-type"></a>managementagenttype 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理エージェントの種類。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|eas|1-d|デバイスは、Exchange server によって管理されています。|
|mdm.exe|pbm-2|デバイスは Intune MDM によって管理されます。|
|easmdm|1/3|デバイスは、Exchange server と Intune MDM の両方によって管理されます。|
|intアンの場合|2/4|Intune クライアント管理。|
|easintアンの場合|5|デバイスは EAS で、Intune クライアントはデュアル管理されています。|
|configurationmanagerclient|~|デバイスは構成マネージャーによって管理されています。|
|configurationmanagerclientmdm|個|デバイスは、構成マネージャーおよび MDM によって管理されます。|
|configurationmanagerclientmdmeas|#|デバイスは、構成マネージャー、MDM、Eas によって管理されます。|
|不明|16|管理エージェントの種類が不明です。|
|jamf|32|デバイス属性は、Jamf から取得されます。|
|googleCloudDevicePolicyController|64|デバイスは Google の CloudDPC によって管理されています。|



