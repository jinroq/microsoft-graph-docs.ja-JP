---
title: numberRange リソースの種類
description: 番号範囲の定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbc802ef17c6e83d10f93661e7aca05cdc2cee02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969983"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="7e857-103">numberRange リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e857-103">numberRange resource type</span></span>

> <span data-ttu-id="7e857-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e857-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e857-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e857-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e857-106">番号範囲の定義。</span><span class="sxs-lookup"><span data-stu-id="7e857-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7e857-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e857-107">Properties</span></span>
|<span data-ttu-id="7e857-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e857-108">Property</span></span>|<span data-ttu-id="7e857-109">型</span><span class="sxs-lookup"><span data-stu-id="7e857-109">Type</span></span>|<span data-ttu-id="7e857-110">説明</span><span class="sxs-lookup"><span data-stu-id="7e857-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e857-111">小数</span><span class="sxs-lookup"><span data-stu-id="7e857-111">lowerNumber</span></span>|<span data-ttu-id="7e857-112">Int32</span><span class="sxs-lookup"><span data-stu-id="7e857-112">Int32</span></span>|<span data-ttu-id="7e857-113">数値 (小)</span><span class="sxs-lookup"><span data-stu-id="7e857-113">Lower number.</span></span>|
|<span data-ttu-id="7e857-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="7e857-114">upperNumber</span></span>|<span data-ttu-id="7e857-115">Int32</span><span class="sxs-lookup"><span data-stu-id="7e857-115">Int32</span></span>|<span data-ttu-id="7e857-116">上番号</span><span class="sxs-lookup"><span data-stu-id="7e857-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e857-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e857-117">Relationships</span></span>
<span data-ttu-id="7e857-118">なし</span><span class="sxs-lookup"><span data-stu-id="7e857-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e857-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e857-119">JSON Representation</span></span>
<span data-ttu-id="7e857-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e857-120">Here is a JSON representation of the resource.</span></span>
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





