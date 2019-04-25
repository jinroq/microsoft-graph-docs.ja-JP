---
title: numberRange リソースの種類
description: 番号範囲の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 225dc4a48e0f95ccf1fdeae828c1ec603ed68802
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542278"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="bb4b2-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb4b2-103">numberRange resource type</span></span>

> <span data-ttu-id="bb4b2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb4b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb4b2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb4b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4b2-106">番号範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="bb4b2-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bb4b2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb4b2-107">Properties</span></span>
|<span data-ttu-id="bb4b2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb4b2-108">Property</span></span>|<span data-ttu-id="bb4b2-109">型</span><span class="sxs-lookup"><span data-stu-id="bb4b2-109">Type</span></span>|<span data-ttu-id="bb4b2-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb4b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4b2-111">小数</span><span class="sxs-lookup"><span data-stu-id="bb4b2-111">lowerNumber</span></span>|<span data-ttu-id="bb4b2-112">Int32</span><span class="sxs-lookup"><span data-stu-id="bb4b2-112">Int32</span></span>|<span data-ttu-id="bb4b2-113">数値 (小)</span><span class="sxs-lookup"><span data-stu-id="bb4b2-113">Lower number.</span></span>|
|<span data-ttu-id="bb4b2-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="bb4b2-114">upperNumber</span></span>|<span data-ttu-id="bb4b2-115">Int32</span><span class="sxs-lookup"><span data-stu-id="bb4b2-115">Int32</span></span>|<span data-ttu-id="bb4b2-116">上番号</span><span class="sxs-lookup"><span data-stu-id="bb4b2-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb4b2-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb4b2-117">Relationships</span></span>
<span data-ttu-id="bb4b2-118">なし</span><span class="sxs-lookup"><span data-stu-id="bb4b2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb4b2-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb4b2-119">JSON Representation</span></span>
<span data-ttu-id="bb4b2-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb4b2-120">Here is a JSON representation of the resource.</span></span>
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





