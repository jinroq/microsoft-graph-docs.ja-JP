---
title: deviceActionResult リソースの種類
description: デバイス アクションの結果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 518d0d09d7ef4f9fea67ce8d600f97be0345fa63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404709"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="ce8a9-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce8a9-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="ce8a9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce8a9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce8a9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce8a9-107">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ce8a9-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="ce8a9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8a9-108">Properties</span></span>
|<span data-ttu-id="ce8a9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8a9-109">Property</span></span>|<span data-ttu-id="ce8a9-110">型</span><span class="sxs-lookup"><span data-stu-id="ce8a9-110">Type</span></span>|<span data-ttu-id="ce8a9-111">説明</span><span class="sxs-lookup"><span data-stu-id="ce8a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce8a9-112">actionName</span><span class="sxs-lookup"><span data-stu-id="ce8a9-112">actionName</span></span>|<span data-ttu-id="ce8a9-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ce8a9-113">String</span></span>|<span data-ttu-id="ce8a9-114">アクション名</span><span class="sxs-lookup"><span data-stu-id="ce8a9-114">Action name</span></span>|
|<span data-ttu-id="ce8a9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="ce8a9-115">actionState</span></span>|[<span data-ttu-id="ce8a9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ce8a9-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ce8a9-117">アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-117">State of the action.</span></span> <span data-ttu-id="ce8a9-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ce8a9-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8a9-119">startDateTime</span></span>|<span data-ttu-id="ce8a9-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8a9-120">DateTimeOffset</span></span>|<span data-ttu-id="ce8a9-121">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="ce8a9-121">Time the action was initiated</span></span>|
|<span data-ttu-id="ce8a9-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8a9-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="ce8a9-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8a9-123">DateTimeOffset</span></span>|<span data-ttu-id="ce8a9-124">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="ce8a9-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce8a9-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce8a9-125">Relationships</span></span>
<span data-ttu-id="ce8a9-126">なし</span><span class="sxs-lookup"><span data-stu-id="ce8a9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce8a9-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce8a9-127">JSON Representation</span></span>
<span data-ttu-id="ce8a9-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




