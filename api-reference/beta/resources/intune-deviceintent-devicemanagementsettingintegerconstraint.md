---
title: Devicemanagementsetting整数制約リソースの種類
description: 整数設定に許可されている値の範囲を適用する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d934da42efdfed3f161e11c0fc9835191e2051
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984500"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="558de-103">Devicemanagementsetting整数制約リソースの種類</span><span class="sxs-lookup"><span data-stu-id="558de-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="558de-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="558de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="558de-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="558de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="558de-106">整数設定に許可されている値の範囲を適用する制約</span><span class="sxs-lookup"><span data-stu-id="558de-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="558de-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="558de-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="558de-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="558de-108">Properties</span></span>
|<span data-ttu-id="558de-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="558de-109">Property</span></span>|<span data-ttu-id="558de-110">型</span><span class="sxs-lookup"><span data-stu-id="558de-110">Type</span></span>|<span data-ttu-id="558de-111">説明</span><span class="sxs-lookup"><span data-stu-id="558de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558de-112">minimumValue</span><span class="sxs-lookup"><span data-stu-id="558de-112">minimumValue</span></span>|<span data-ttu-id="558de-113">Int32</span><span class="sxs-lookup"><span data-stu-id="558de-113">Int32</span></span>|<span data-ttu-id="558de-114">許可される最小値</span><span class="sxs-lookup"><span data-stu-id="558de-114">The minimum permitted value</span></span>|
|<span data-ttu-id="558de-115">maximumValue</span><span class="sxs-lookup"><span data-stu-id="558de-115">maximumValue</span></span>|<span data-ttu-id="558de-116">Int32</span><span class="sxs-lookup"><span data-stu-id="558de-116">Int32</span></span>|<span data-ttu-id="558de-117">許可される最大値</span><span class="sxs-lookup"><span data-stu-id="558de-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="558de-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="558de-118">Relationships</span></span>
<span data-ttu-id="558de-119">なし</span><span class="sxs-lookup"><span data-stu-id="558de-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="558de-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="558de-120">JSON Representation</span></span>
<span data-ttu-id="558de-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="558de-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```





