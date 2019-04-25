---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565801"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="9eba7-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9eba7-103">auditProperty resource type</span></span>

> <span data-ttu-id="9eba7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9eba7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eba7-105">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="9eba7-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="9eba7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9eba7-106">Properties</span></span>
|<span data-ttu-id="9eba7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9eba7-107">Property</span></span>|<span data-ttu-id="9eba7-108">型</span><span class="sxs-lookup"><span data-stu-id="9eba7-108">Type</span></span>|<span data-ttu-id="9eba7-109">説明</span><span class="sxs-lookup"><span data-stu-id="9eba7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eba7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9eba7-110">displayName</span></span>|<span data-ttu-id="9eba7-111">String</span><span class="sxs-lookup"><span data-stu-id="9eba7-111">String</span></span>|<span data-ttu-id="9eba7-112">表示名。</span><span class="sxs-lookup"><span data-stu-id="9eba7-112">Display name.</span></span>|
|<span data-ttu-id="9eba7-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="9eba7-113">oldValue</span></span>|<span data-ttu-id="9eba7-114">String</span><span class="sxs-lookup"><span data-stu-id="9eba7-114">String</span></span>|<span data-ttu-id="9eba7-115">以前の値。</span><span class="sxs-lookup"><span data-stu-id="9eba7-115">Old value.</span></span>|
|<span data-ttu-id="9eba7-116">newValue</span><span class="sxs-lookup"><span data-stu-id="9eba7-116">newValue</span></span>|<span data-ttu-id="9eba7-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9eba7-117">String</span></span>|<span data-ttu-id="9eba7-118">新しい値。</span><span class="sxs-lookup"><span data-stu-id="9eba7-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eba7-119">関係</span><span class="sxs-lookup"><span data-stu-id="9eba7-119">Relationships</span></span>
<span data-ttu-id="9eba7-120">なし</span><span class="sxs-lookup"><span data-stu-id="9eba7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9eba7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9eba7-121">JSON Representation</span></span>
<span data-ttu-id="9eba7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9eba7-122">Here is a JSON representation of the resource.</span></span>
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



