---
title: numberRange リソースの種類
description: 番号範囲の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711206a256e17d6e10c7c54cf8a3dda4868db031
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166788"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="114d0-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="114d0-103">numberRange resource type</span></span>

> <span data-ttu-id="114d0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="114d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="114d0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="114d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="114d0-106">番号範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="114d0-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="114d0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="114d0-107">Properties</span></span>
|<span data-ttu-id="114d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="114d0-108">Property</span></span>|<span data-ttu-id="114d0-109">型</span><span class="sxs-lookup"><span data-stu-id="114d0-109">Type</span></span>|<span data-ttu-id="114d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="114d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="114d0-111">小数</span><span class="sxs-lookup"><span data-stu-id="114d0-111">lowerNumber</span></span>|<span data-ttu-id="114d0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="114d0-112">Int32</span></span>|<span data-ttu-id="114d0-113">数値 (小)</span><span class="sxs-lookup"><span data-stu-id="114d0-113">Lower number.</span></span>|
|<span data-ttu-id="114d0-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="114d0-114">upperNumber</span></span>|<span data-ttu-id="114d0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="114d0-115">Int32</span></span>|<span data-ttu-id="114d0-116">上番号</span><span class="sxs-lookup"><span data-stu-id="114d0-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="114d0-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="114d0-117">Relationships</span></span>
<span data-ttu-id="114d0-118">なし</span><span class="sxs-lookup"><span data-stu-id="114d0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="114d0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="114d0-119">JSON Representation</span></span>
<span data-ttu-id="114d0-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="114d0-120">Here is a JSON representation of the resource.</span></span>
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




