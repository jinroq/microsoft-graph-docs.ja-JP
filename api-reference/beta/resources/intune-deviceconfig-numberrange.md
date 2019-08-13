---
title: numberRange リソースの種類
description: 番号範囲の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b300f3d0db3a2a310d0a19408750b1dd9ac5c46
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368549"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="b674f-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b674f-103">numberRange resource type</span></span>

> <span data-ttu-id="b674f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b674f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b674f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b674f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b674f-106">番号範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="b674f-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b674f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b674f-107">Properties</span></span>
|<span data-ttu-id="b674f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b674f-108">Property</span></span>|<span data-ttu-id="b674f-109">型</span><span class="sxs-lookup"><span data-stu-id="b674f-109">Type</span></span>|<span data-ttu-id="b674f-110">説明</span><span class="sxs-lookup"><span data-stu-id="b674f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b674f-111">小数</span><span class="sxs-lookup"><span data-stu-id="b674f-111">lowerNumber</span></span>|<span data-ttu-id="b674f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b674f-112">Int32</span></span>|<span data-ttu-id="b674f-113">数値 (小)</span><span class="sxs-lookup"><span data-stu-id="b674f-113">Lower number.</span></span>|
|<span data-ttu-id="b674f-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="b674f-114">upperNumber</span></span>|<span data-ttu-id="b674f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b674f-115">Int32</span></span>|<span data-ttu-id="b674f-116">上番号</span><span class="sxs-lookup"><span data-stu-id="b674f-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b674f-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b674f-117">Relationships</span></span>
<span data-ttu-id="b674f-118">なし</span><span class="sxs-lookup"><span data-stu-id="b674f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b674f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b674f-119">JSON Representation</span></span>
<span data-ttu-id="b674f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b674f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```



