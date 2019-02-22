---
title: keyValue リソースの種類
description: キー値の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597f6d2101e4549336693f1cff7ce64199b46287
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155497"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="8b2a7-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8b2a7-103">keyValue resource type</span></span>

> <span data-ttu-id="8b2a7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b2a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b2a7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b2a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b2a7-106">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="8b2a7-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8b2a7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2a7-107">Properties</span></span>
|<span data-ttu-id="8b2a7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2a7-108">Property</span></span>|<span data-ttu-id="8b2a7-109">型</span><span class="sxs-lookup"><span data-stu-id="8b2a7-109">Type</span></span>|<span data-ttu-id="8b2a7-110">説明</span><span class="sxs-lookup"><span data-stu-id="8b2a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b2a7-111">Key</span><span class="sxs-lookup"><span data-stu-id="8b2a7-111">key</span></span>|<span data-ttu-id="8b2a7-112">String</span><span class="sxs-lookup"><span data-stu-id="8b2a7-112">String</span></span>|<span data-ttu-id="8b2a7-113">キー。</span><span class="sxs-lookup"><span data-stu-id="8b2a7-113">Key.</span></span>|
|<span data-ttu-id="8b2a7-114">value</span><span class="sxs-lookup"><span data-stu-id="8b2a7-114">value</span></span>|<span data-ttu-id="8b2a7-115">文字列</span><span class="sxs-lookup"><span data-stu-id="8b2a7-115">String</span></span>|<span data-ttu-id="8b2a7-116">値。</span><span class="sxs-lookup"><span data-stu-id="8b2a7-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b2a7-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8b2a7-117">Relationships</span></span>
<span data-ttu-id="8b2a7-118">なし</span><span class="sxs-lookup"><span data-stu-id="8b2a7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b2a7-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8b2a7-119">JSON Representation</span></span>
<span data-ttu-id="8b2a7-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8b2a7-120">Here is a JSON representation of the resource.</span></span>
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




