---
title: numberRange リソースの種類
description: 番号範囲の定義です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27393bdac6519078c2021e3484ae58ddf43216d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416861"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="75909-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75909-103">numberRange resource type</span></span>

> <span data-ttu-id="75909-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75909-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="75909-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75909-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75909-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75909-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75909-107">番号範囲の定義です。</span><span class="sxs-lookup"><span data-stu-id="75909-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="75909-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75909-108">Properties</span></span>
|<span data-ttu-id="75909-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75909-109">Property</span></span>|<span data-ttu-id="75909-110">型</span><span class="sxs-lookup"><span data-stu-id="75909-110">Type</span></span>|<span data-ttu-id="75909-111">説明</span><span class="sxs-lookup"><span data-stu-id="75909-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75909-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="75909-112">lowerNumber</span></span>|<span data-ttu-id="75909-113">Int32</span><span class="sxs-lookup"><span data-stu-id="75909-113">Int32</span></span>|<span data-ttu-id="75909-114">下の数です。</span><span class="sxs-lookup"><span data-stu-id="75909-114">Lower number.</span></span>|
|<span data-ttu-id="75909-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="75909-115">upperNumber</span></span>|<span data-ttu-id="75909-116">Int32</span><span class="sxs-lookup"><span data-stu-id="75909-116">Int32</span></span>|<span data-ttu-id="75909-117">上の数です。</span><span class="sxs-lookup"><span data-stu-id="75909-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75909-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75909-118">Relationships</span></span>
<span data-ttu-id="75909-119">なし</span><span class="sxs-lookup"><span data-stu-id="75909-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75909-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75909-120">JSON Representation</span></span>
<span data-ttu-id="75909-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75909-121">Here is a JSON representation of the resource.</span></span>
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




