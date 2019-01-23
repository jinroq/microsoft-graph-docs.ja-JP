---
title: keyValue リソースの種類
description: キー値の定義。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e3133962d9f6bfb5f5363dd6d6cbd4b5ef2ea202
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406816"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="0a090-103">keyValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a090-103">keyValue resource type</span></span>

> <span data-ttu-id="0a090-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a090-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0a090-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a090-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a090-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a090-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a090-107">キー値の定義。</span><span class="sxs-lookup"><span data-stu-id="0a090-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0a090-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a090-108">Properties</span></span>
|<span data-ttu-id="0a090-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a090-109">Property</span></span>|<span data-ttu-id="0a090-110">型</span><span class="sxs-lookup"><span data-stu-id="0a090-110">Type</span></span>|<span data-ttu-id="0a090-111">説明</span><span class="sxs-lookup"><span data-stu-id="0a090-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a090-112">Key</span><span class="sxs-lookup"><span data-stu-id="0a090-112">key</span></span>|<span data-ttu-id="0a090-113">String</span><span class="sxs-lookup"><span data-stu-id="0a090-113">String</span></span>|<span data-ttu-id="0a090-114">キー。</span><span class="sxs-lookup"><span data-stu-id="0a090-114">Key.</span></span>|
|<span data-ttu-id="0a090-115">value</span><span class="sxs-lookup"><span data-stu-id="0a090-115">value</span></span>|<span data-ttu-id="0a090-116">文字列</span><span class="sxs-lookup"><span data-stu-id="0a090-116">String</span></span>|<span data-ttu-id="0a090-117">値。</span><span class="sxs-lookup"><span data-stu-id="0a090-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a090-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a090-118">Relationships</span></span>
<span data-ttu-id="0a090-119">なし</span><span class="sxs-lookup"><span data-stu-id="0a090-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a090-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a090-120">JSON Representation</span></span>
<span data-ttu-id="0a090-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a090-121">Here is a JSON representation of the resource.</span></span>
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




