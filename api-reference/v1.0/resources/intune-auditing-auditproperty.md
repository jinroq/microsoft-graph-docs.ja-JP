---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260614"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="3a2b5-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a2b5-103">auditProperty resource type</span></span>

> <span data-ttu-id="3a2b5-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3a2b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a2b5-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="3a2b5-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="3a2b5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a2b5-106">Properties</span></span>
|<span data-ttu-id="3a2b5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a2b5-107">Property</span></span>|<span data-ttu-id="3a2b5-108">型</span><span class="sxs-lookup"><span data-stu-id="3a2b5-108">Type</span></span>|<span data-ttu-id="3a2b5-109">説明</span><span class="sxs-lookup"><span data-stu-id="3a2b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a2b5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3a2b5-110">displayName</span></span>|<span data-ttu-id="3a2b5-111">String</span><span class="sxs-lookup"><span data-stu-id="3a2b5-111">String</span></span>|<span data-ttu-id="3a2b5-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="3a2b5-112">Display name.</span></span>|
|<span data-ttu-id="3a2b5-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="3a2b5-113">oldValue</span></span>|<span data-ttu-id="3a2b5-114">String</span><span class="sxs-lookup"><span data-stu-id="3a2b5-114">String</span></span>|<span data-ttu-id="3a2b5-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="3a2b5-115">Old value.</span></span>|
|<span data-ttu-id="3a2b5-116">newValue</span><span class="sxs-lookup"><span data-stu-id="3a2b5-116">newValue</span></span>|<span data-ttu-id="3a2b5-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3a2b5-117">String</span></span>|<span data-ttu-id="3a2b5-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="3a2b5-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a2b5-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3a2b5-119">Relationships</span></span>
<span data-ttu-id="3a2b5-120">なし</span><span class="sxs-lookup"><span data-stu-id="3a2b5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a2b5-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a2b5-121">JSON Representation</span></span>
<span data-ttu-id="3a2b5-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a2b5-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



