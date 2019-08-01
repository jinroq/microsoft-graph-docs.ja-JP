---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a3e4ed10a756c4d1cb62bf98c1b6cb13d6f22c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032054"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="76157-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76157-103">auditProperty resource type</span></span>

> <span data-ttu-id="76157-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76157-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76157-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="76157-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="76157-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76157-106">Properties</span></span>
|<span data-ttu-id="76157-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76157-107">Property</span></span>|<span data-ttu-id="76157-108">型</span><span class="sxs-lookup"><span data-stu-id="76157-108">Type</span></span>|<span data-ttu-id="76157-109">説明</span><span class="sxs-lookup"><span data-stu-id="76157-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76157-110">displayName</span><span class="sxs-lookup"><span data-stu-id="76157-110">displayName</span></span>|<span data-ttu-id="76157-111">String</span><span class="sxs-lookup"><span data-stu-id="76157-111">String</span></span>|<span data-ttu-id="76157-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="76157-112">Display name.</span></span>|
|<span data-ttu-id="76157-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="76157-113">oldValue</span></span>|<span data-ttu-id="76157-114">String</span><span class="sxs-lookup"><span data-stu-id="76157-114">String</span></span>|<span data-ttu-id="76157-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="76157-115">Old value.</span></span>|
|<span data-ttu-id="76157-116">newValue</span><span class="sxs-lookup"><span data-stu-id="76157-116">newValue</span></span>|<span data-ttu-id="76157-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="76157-117">String</span></span>|<span data-ttu-id="76157-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="76157-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76157-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76157-119">Relationships</span></span>
<span data-ttu-id="76157-120">なし</span><span class="sxs-lookup"><span data-stu-id="76157-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76157-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76157-121">JSON Representation</span></span>
<span data-ttu-id="76157-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76157-122">Here is a JSON representation of the resource.</span></span>
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



