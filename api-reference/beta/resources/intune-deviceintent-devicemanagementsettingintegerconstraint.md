---
title: devicemanagementsetting整数制約リソースの種類
description: 整数設定に許可されている値の範囲を適用する制約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bf28c3f3942e99841b43f1cd7ff5304fd81d800
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781261"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="4f841-103">devicemanagementsetting整数制約リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f841-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="4f841-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f841-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f841-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4f841-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f841-106">整数設定に許可されている値の範囲を適用する制約</span><span class="sxs-lookup"><span data-stu-id="4f841-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="4f841-107">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="4f841-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f841-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f841-108">Properties</span></span>
|<span data-ttu-id="4f841-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f841-109">Property</span></span>|<span data-ttu-id="4f841-110">型</span><span class="sxs-lookup"><span data-stu-id="4f841-110">Type</span></span>|<span data-ttu-id="4f841-111">説明</span><span class="sxs-lookup"><span data-stu-id="4f841-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f841-112">minimumvalue</span><span class="sxs-lookup"><span data-stu-id="4f841-112">minimumValue</span></span>|<span data-ttu-id="4f841-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4f841-113">Int32</span></span>|<span data-ttu-id="4f841-114">許可される最小値</span><span class="sxs-lookup"><span data-stu-id="4f841-114">The minimum permitted value</span></span>|
|<span data-ttu-id="4f841-115">maximumValue</span><span class="sxs-lookup"><span data-stu-id="4f841-115">maximumValue</span></span>|<span data-ttu-id="4f841-116">Int32</span><span class="sxs-lookup"><span data-stu-id="4f841-116">Int32</span></span>|<span data-ttu-id="4f841-117">許可される最大値</span><span class="sxs-lookup"><span data-stu-id="4f841-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f841-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4f841-118">Relationships</span></span>
<span data-ttu-id="4f841-119">なし</span><span class="sxs-lookup"><span data-stu-id="4f841-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f841-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f841-120">JSON Representation</span></span>
<span data-ttu-id="4f841-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4f841-121">Here is a JSON representation of the resource.</span></span>
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





