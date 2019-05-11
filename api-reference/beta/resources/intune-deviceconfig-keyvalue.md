---
title: keyValue リソースの種類
description: キー値の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 592f3ff070ab7440d5c16d5380b556993915e6ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946124"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="52f46-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52f46-103">keyValue resource type</span></span>

> <span data-ttu-id="52f46-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52f46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52f46-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52f46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52f46-106">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="52f46-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="52f46-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52f46-107">Properties</span></span>
|<span data-ttu-id="52f46-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52f46-108">Property</span></span>|<span data-ttu-id="52f46-109">型</span><span class="sxs-lookup"><span data-stu-id="52f46-109">Type</span></span>|<span data-ttu-id="52f46-110">説明</span><span class="sxs-lookup"><span data-stu-id="52f46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f46-111">Key</span><span class="sxs-lookup"><span data-stu-id="52f46-111">key</span></span>|<span data-ttu-id="52f46-112">String</span><span class="sxs-lookup"><span data-stu-id="52f46-112">String</span></span>|<span data-ttu-id="52f46-113">キー。</span><span class="sxs-lookup"><span data-stu-id="52f46-113">Key.</span></span>|
|<span data-ttu-id="52f46-114">value</span><span class="sxs-lookup"><span data-stu-id="52f46-114">value</span></span>|<span data-ttu-id="52f46-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="52f46-115">String</span></span>|<span data-ttu-id="52f46-116">値。</span><span class="sxs-lookup"><span data-stu-id="52f46-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52f46-117">関係</span><span class="sxs-lookup"><span data-stu-id="52f46-117">Relationships</span></span>
<span data-ttu-id="52f46-118">なし</span><span class="sxs-lookup"><span data-stu-id="52f46-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52f46-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52f46-119">JSON Representation</span></span>
<span data-ttu-id="52f46-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52f46-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




