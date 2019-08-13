---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 331c786d7fd21687a0581ae56746d9e0b48f7c04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335229"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="48ddb-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48ddb-103">auditProperty resource type</span></span>

> <span data-ttu-id="48ddb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48ddb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48ddb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48ddb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48ddb-106">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="48ddb-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="48ddb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48ddb-107">Properties</span></span>
|<span data-ttu-id="48ddb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48ddb-108">Property</span></span>|<span data-ttu-id="48ddb-109">型</span><span class="sxs-lookup"><span data-stu-id="48ddb-109">Type</span></span>|<span data-ttu-id="48ddb-110">説明</span><span class="sxs-lookup"><span data-stu-id="48ddb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48ddb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="48ddb-111">displayName</span></span>|<span data-ttu-id="48ddb-112">String</span><span class="sxs-lookup"><span data-stu-id="48ddb-112">String</span></span>|<span data-ttu-id="48ddb-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="48ddb-113">Display name.</span></span>|
|<span data-ttu-id="48ddb-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="48ddb-114">oldValue</span></span>|<span data-ttu-id="48ddb-115">String</span><span class="sxs-lookup"><span data-stu-id="48ddb-115">String</span></span>|<span data-ttu-id="48ddb-116">以前の値。</span><span class="sxs-lookup"><span data-stu-id="48ddb-116">Old value.</span></span>|
|<span data-ttu-id="48ddb-117">newValue</span><span class="sxs-lookup"><span data-stu-id="48ddb-117">newValue</span></span>|<span data-ttu-id="48ddb-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="48ddb-118">String</span></span>|<span data-ttu-id="48ddb-119">新しい値。</span><span class="sxs-lookup"><span data-stu-id="48ddb-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48ddb-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48ddb-120">Relationships</span></span>
<span data-ttu-id="48ddb-121">なし</span><span class="sxs-lookup"><span data-stu-id="48ddb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48ddb-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48ddb-122">JSON Representation</span></span>
<span data-ttu-id="48ddb-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48ddb-123">Here is a JSON representation of the resource.</span></span>
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



