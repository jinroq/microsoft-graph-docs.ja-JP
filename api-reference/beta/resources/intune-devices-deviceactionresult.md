---
title: deviceActionResult リソースの種類
description: デバイスのアクションの結果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d46aa2d4359430d17e3f3892b8b526a9efed603
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523337"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="1f46e-103">deviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f46e-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="1f46e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f46e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f46e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1f46e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f46e-106">デバイス アクションの結果</span><span class="sxs-lookup"><span data-stu-id="1f46e-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="1f46e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f46e-107">Properties</span></span>
|<span data-ttu-id="1f46e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f46e-108">Property</span></span>|<span data-ttu-id="1f46e-109">型</span><span class="sxs-lookup"><span data-stu-id="1f46e-109">Type</span></span>|<span data-ttu-id="1f46e-110">説明</span><span class="sxs-lookup"><span data-stu-id="1f46e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f46e-111">actionName</span><span class="sxs-lookup"><span data-stu-id="1f46e-111">actionName</span></span>|<span data-ttu-id="1f46e-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1f46e-112">String</span></span>|<span data-ttu-id="1f46e-113">アクション名</span><span class="sxs-lookup"><span data-stu-id="1f46e-113">Action name</span></span>|
|<span data-ttu-id="1f46e-114">actionState</span><span class="sxs-lookup"><span data-stu-id="1f46e-114">actionState</span></span>|[<span data-ttu-id="1f46e-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1f46e-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1f46e-116">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="1f46e-116">State of the action.</span></span> <span data-ttu-id="1f46e-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="1f46e-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1f46e-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1f46e-118">startDateTime</span></span>|<span data-ttu-id="1f46e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f46e-119">DateTimeOffset</span></span>|<span data-ttu-id="1f46e-120">アクションが開始された時刻</span><span class="sxs-lookup"><span data-stu-id="1f46e-120">Time the action was initiated</span></span>|
|<span data-ttu-id="1f46e-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f46e-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="1f46e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f46e-122">DateTimeOffset</span></span>|<span data-ttu-id="1f46e-123">アクション状態の最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="1f46e-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f46e-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f46e-124">Relationships</span></span>
<span data-ttu-id="1f46e-125">なし</span><span class="sxs-lookup"><span data-stu-id="1f46e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f46e-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f46e-126">JSON Representation</span></span>
<span data-ttu-id="1f46e-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1f46e-127">Here is a JSON representation of the resource.</span></span>
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





