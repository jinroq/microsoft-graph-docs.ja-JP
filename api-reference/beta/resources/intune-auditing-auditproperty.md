---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27eda22c48f60da1cd224add29559b13505f7d8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004877"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="d3162-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3162-103">auditProperty resource type</span></span>

> <span data-ttu-id="d3162-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3162-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3162-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3162-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3162-106">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="d3162-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="d3162-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3162-107">Properties</span></span>
|<span data-ttu-id="d3162-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3162-108">Property</span></span>|<span data-ttu-id="d3162-109">型</span><span class="sxs-lookup"><span data-stu-id="d3162-109">Type</span></span>|<span data-ttu-id="d3162-110">説明</span><span class="sxs-lookup"><span data-stu-id="d3162-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3162-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d3162-111">displayName</span></span>|<span data-ttu-id="d3162-112">String</span><span class="sxs-lookup"><span data-stu-id="d3162-112">String</span></span>|<span data-ttu-id="d3162-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="d3162-113">Display name.</span></span>|
|<span data-ttu-id="d3162-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="d3162-114">oldValue</span></span>|<span data-ttu-id="d3162-115">String</span><span class="sxs-lookup"><span data-stu-id="d3162-115">String</span></span>|<span data-ttu-id="d3162-116">以前の値。</span><span class="sxs-lookup"><span data-stu-id="d3162-116">Old value.</span></span>|
|<span data-ttu-id="d3162-117">newValue</span><span class="sxs-lookup"><span data-stu-id="d3162-117">newValue</span></span>|<span data-ttu-id="d3162-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d3162-118">String</span></span>|<span data-ttu-id="d3162-119">新しい値。</span><span class="sxs-lookup"><span data-stu-id="d3162-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3162-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3162-120">Relationships</span></span>
<span data-ttu-id="d3162-121">なし</span><span class="sxs-lookup"><span data-stu-id="d3162-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3162-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3162-122">JSON Representation</span></span>
<span data-ttu-id="d3162-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3162-123">Here is a JSON representation of the resource.</span></span>
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





