---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3425c59ae4f30b30b04bd22f74cb1b27ad99191f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416644"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="0547a-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0547a-103">auditProperty resource type</span></span>

> <span data-ttu-id="0547a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0547a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0547a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0547a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0547a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0547a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0547a-107">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="0547a-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="0547a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0547a-108">Properties</span></span>
|<span data-ttu-id="0547a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0547a-109">Property</span></span>|<span data-ttu-id="0547a-110">型</span><span class="sxs-lookup"><span data-stu-id="0547a-110">Type</span></span>|<span data-ttu-id="0547a-111">説明</span><span class="sxs-lookup"><span data-stu-id="0547a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0547a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0547a-112">displayName</span></span>|<span data-ttu-id="0547a-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0547a-113">String</span></span>|<span data-ttu-id="0547a-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="0547a-114">Display name.</span></span>|
|<span data-ttu-id="0547a-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="0547a-115">oldValue</span></span>|<span data-ttu-id="0547a-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0547a-116">String</span></span>|<span data-ttu-id="0547a-117">以前の値。</span><span class="sxs-lookup"><span data-stu-id="0547a-117">Old value.</span></span>|
|<span data-ttu-id="0547a-118">newValue</span><span class="sxs-lookup"><span data-stu-id="0547a-118">newValue</span></span>|<span data-ttu-id="0547a-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0547a-119">String</span></span>|<span data-ttu-id="0547a-120">新しい値。</span><span class="sxs-lookup"><span data-stu-id="0547a-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0547a-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0547a-121">Relationships</span></span>
<span data-ttu-id="0547a-122">なし</span><span class="sxs-lookup"><span data-stu-id="0547a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0547a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0547a-123">JSON Representation</span></span>
<span data-ttu-id="0547a-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0547a-124">Here is a JSON representation of the resource.</span></span>
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




