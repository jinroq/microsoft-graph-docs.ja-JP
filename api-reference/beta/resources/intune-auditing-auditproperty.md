---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c252e7912f3f34e300e1f412db63133ea3acbd8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949361"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="8c496-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c496-103">auditProperty resource type</span></span>

> <span data-ttu-id="8c496-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c496-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c496-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c496-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c496-106">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="8c496-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="8c496-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c496-107">Properties</span></span>
|<span data-ttu-id="8c496-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c496-108">Property</span></span>|<span data-ttu-id="8c496-109">型</span><span class="sxs-lookup"><span data-stu-id="8c496-109">Type</span></span>|<span data-ttu-id="8c496-110">説明</span><span class="sxs-lookup"><span data-stu-id="8c496-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c496-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8c496-111">displayName</span></span>|<span data-ttu-id="8c496-112">String</span><span class="sxs-lookup"><span data-stu-id="8c496-112">String</span></span>|<span data-ttu-id="8c496-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="8c496-113">Display name.</span></span>|
|<span data-ttu-id="8c496-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="8c496-114">oldValue</span></span>|<span data-ttu-id="8c496-115">String</span><span class="sxs-lookup"><span data-stu-id="8c496-115">String</span></span>|<span data-ttu-id="8c496-116">以前の値。</span><span class="sxs-lookup"><span data-stu-id="8c496-116">Old value.</span></span>|
|<span data-ttu-id="8c496-117">newValue</span><span class="sxs-lookup"><span data-stu-id="8c496-117">newValue</span></span>|<span data-ttu-id="8c496-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8c496-118">String</span></span>|<span data-ttu-id="8c496-119">新しい値。</span><span class="sxs-lookup"><span data-stu-id="8c496-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c496-120">関係</span><span class="sxs-lookup"><span data-stu-id="8c496-120">Relationships</span></span>
<span data-ttu-id="8c496-121">なし</span><span class="sxs-lookup"><span data-stu-id="8c496-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c496-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c496-122">JSON Representation</span></span>
<span data-ttu-id="8c496-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c496-123">Here is a JSON representation of the resource.</span></span>
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




