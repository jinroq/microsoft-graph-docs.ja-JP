---
title: deviceActionResult リソースの種類
description: デバイスのアクションの結果
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58f8c4b435328d700a2d5e83a0c111738f6cad75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968513"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="be63b-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be63b-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="be63b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be63b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be63b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be63b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be63b-106">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="be63b-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="be63b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be63b-107">Properties</span></span>
|<span data-ttu-id="be63b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be63b-108">Property</span></span>|<span data-ttu-id="be63b-109">型</span><span class="sxs-lookup"><span data-stu-id="be63b-109">Type</span></span>|<span data-ttu-id="be63b-110">説明</span><span class="sxs-lookup"><span data-stu-id="be63b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be63b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="be63b-111">actionName</span></span>|<span data-ttu-id="be63b-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="be63b-112">String</span></span>|<span data-ttu-id="be63b-113">アクション名</span><span class="sxs-lookup"><span data-stu-id="be63b-113">Action name</span></span>|
|<span data-ttu-id="be63b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="be63b-114">actionState</span></span>|[<span data-ttu-id="be63b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="be63b-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="be63b-116">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="be63b-116">State of the action.</span></span> <span data-ttu-id="be63b-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="be63b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="be63b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="be63b-118">startDateTime</span></span>|<span data-ttu-id="be63b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be63b-119">DateTimeOffset</span></span>|<span data-ttu-id="be63b-120">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="be63b-120">Time the action was initiated</span></span>|
|<span data-ttu-id="be63b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="be63b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="be63b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be63b-122">DateTimeOffset</span></span>|<span data-ttu-id="be63b-123">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="be63b-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="be63b-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be63b-124">Relationships</span></span>
<span data-ttu-id="be63b-125">なし</span><span class="sxs-lookup"><span data-stu-id="be63b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be63b-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be63b-126">JSON Representation</span></span>
<span data-ttu-id="be63b-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be63b-127">Here is a JSON representation of the resource.</span></span>
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





