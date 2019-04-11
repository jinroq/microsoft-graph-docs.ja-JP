---
title: auditProperty リソースの種類
description: 監査のプロパティのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f864f41a2068d6455dccb0a539c14e7e4b9dc6d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792763"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="d5360-103">auditProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5360-103">auditProperty resource type</span></span>

> <span data-ttu-id="d5360-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5360-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5360-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5360-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5360-106">監査のプロパティのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="d5360-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="d5360-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5360-107">Properties</span></span>
|<span data-ttu-id="d5360-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5360-108">Property</span></span>|<span data-ttu-id="d5360-109">型</span><span class="sxs-lookup"><span data-stu-id="d5360-109">Type</span></span>|<span data-ttu-id="d5360-110">説明</span><span class="sxs-lookup"><span data-stu-id="d5360-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5360-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d5360-111">displayName</span></span>|<span data-ttu-id="d5360-112">String</span><span class="sxs-lookup"><span data-stu-id="d5360-112">String</span></span>|<span data-ttu-id="d5360-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="d5360-113">Display name.</span></span>|
|<span data-ttu-id="d5360-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="d5360-114">oldValue</span></span>|<span data-ttu-id="d5360-115">文字列</span><span class="sxs-lookup"><span data-stu-id="d5360-115">String</span></span>|<span data-ttu-id="d5360-116">以前の値。</span><span class="sxs-lookup"><span data-stu-id="d5360-116">Old value.</span></span>|
|<span data-ttu-id="d5360-117">newValue</span><span class="sxs-lookup"><span data-stu-id="d5360-117">newValue</span></span>|<span data-ttu-id="d5360-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d5360-118">String</span></span>|<span data-ttu-id="d5360-119">新しい値。</span><span class="sxs-lookup"><span data-stu-id="d5360-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5360-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5360-120">Relationships</span></span>
<span data-ttu-id="d5360-121">なし</span><span class="sxs-lookup"><span data-stu-id="d5360-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5360-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5360-122">JSON Representation</span></span>
<span data-ttu-id="d5360-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d5360-123">Here is a JSON representation of the resource.</span></span>
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





