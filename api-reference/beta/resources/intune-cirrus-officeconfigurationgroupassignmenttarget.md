---
title: officeConfigurationGroupAssignmentTarget リソースの種類
description: Office クライアント構成 AAD グループの割り当て先。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 7458b1071b6133f3b46c8412270e30fdd0bf7638
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949312"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="b0d88-103">officeConfigurationGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0d88-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b0d88-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0d88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0d88-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0d88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0d88-106">Office クライアント構成 AAD グループの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="b0d88-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="b0d88-107">[OfficeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b0d88-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0d88-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0d88-108">Properties</span></span>
|<span data-ttu-id="b0d88-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0d88-109">Property</span></span>|<span data-ttu-id="b0d88-110">型</span><span class="sxs-lookup"><span data-stu-id="b0d88-110">Type</span></span>|<span data-ttu-id="b0d88-111">説明</span><span class="sxs-lookup"><span data-stu-id="b0d88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0d88-112">groupId</span><span class="sxs-lookup"><span data-stu-id="b0d88-112">groupId</span></span>|<span data-ttu-id="b0d88-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0d88-113">String</span></span>|<span data-ttu-id="b0d88-114">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="b0d88-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0d88-115">関係</span><span class="sxs-lookup"><span data-stu-id="b0d88-115">Relationships</span></span>
<span data-ttu-id="b0d88-116">なし</span><span class="sxs-lookup"><span data-stu-id="b0d88-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0d88-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0d88-117">JSON Representation</span></span>
<span data-ttu-id="b0d88-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0d88-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



