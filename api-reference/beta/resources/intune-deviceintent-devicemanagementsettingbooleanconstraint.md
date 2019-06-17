---
title: deviceManagementSettingBooleanConstraint リソースの種類
description: 制約によって特定のブール値が適用されます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 291ee5fa97c0c7b6c77580f2cc55ffce3ff37fdd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963962"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="27a3b-103">deviceManagementSettingBooleanConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27a3b-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="27a3b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27a3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27a3b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27a3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27a3b-106">制約によって特定のブール値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="27a3b-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="27a3b-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="27a3b-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27a3b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27a3b-108">Properties</span></span>
|<span data-ttu-id="27a3b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27a3b-109">Property</span></span>|<span data-ttu-id="27a3b-110">型</span><span class="sxs-lookup"><span data-stu-id="27a3b-110">Type</span></span>|<span data-ttu-id="27a3b-111">説明</span><span class="sxs-lookup"><span data-stu-id="27a3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a3b-112">value</span><span class="sxs-lookup"><span data-stu-id="27a3b-112">value</span></span>|<span data-ttu-id="27a3b-113">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="27a3b-113">Boolean</span></span>|<span data-ttu-id="27a3b-114">比較するブール値</span><span class="sxs-lookup"><span data-stu-id="27a3b-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="27a3b-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="27a3b-115">Relationships</span></span>
<span data-ttu-id="27a3b-116">なし</span><span class="sxs-lookup"><span data-stu-id="27a3b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27a3b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27a3b-117">JSON Representation</span></span>
<span data-ttu-id="27a3b-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27a3b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```





