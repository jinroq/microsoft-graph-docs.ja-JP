---
title: deviceManagementIntentUserStateSummary リソースの種類
description: 目的のユーザー状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b4b13d4dc368c52686aa4d003a0f5995762ec56
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943454"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="96725-103">deviceManagementIntentUserStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96725-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="96725-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96725-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96725-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96725-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96725-106">目的のユーザー状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="96725-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="96725-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="96725-107">Methods</span></span>
|<span data-ttu-id="96725-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="96725-108">Method</span></span>|<span data-ttu-id="96725-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96725-109">Return Type</span></span>|<span data-ttu-id="96725-110">説明</span><span class="sxs-lookup"><span data-stu-id="96725-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96725-111">DeviceManagementIntentUserStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="96725-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="96725-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="96725-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="96725-113">[DeviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96725-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="96725-114">DeviceManagementIntentUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="96725-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="96725-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="96725-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="96725-116">[DeviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="96725-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96725-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96725-117">Properties</span></span>
|<span data-ttu-id="96725-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96725-118">Property</span></span>|<span data-ttu-id="96725-119">型</span><span class="sxs-lookup"><span data-stu-id="96725-119">Type</span></span>|<span data-ttu-id="96725-120">説明</span><span class="sxs-lookup"><span data-stu-id="96725-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96725-121">id</span><span class="sxs-lookup"><span data-stu-id="96725-121">id</span></span>|<span data-ttu-id="96725-122">String</span><span class="sxs-lookup"><span data-stu-id="96725-122">String</span></span>|<span data-ttu-id="96725-123">ID</span><span class="sxs-lookup"><span data-stu-id="96725-123">The ID</span></span>|
|<span data-ttu-id="96725-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="96725-124">conflictCount</span></span>|<span data-ttu-id="96725-125">Int32</span><span class="sxs-lookup"><span data-stu-id="96725-125">Int32</span></span>|<span data-ttu-id="96725-126">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="96725-126">Number of users in conflict</span></span>|
|<span data-ttu-id="96725-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="96725-127">errorCount</span></span>|<span data-ttu-id="96725-128">Int32</span><span class="sxs-lookup"><span data-stu-id="96725-128">Int32</span></span>|<span data-ttu-id="96725-129">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="96725-129">Number of error users</span></span>|
|<span data-ttu-id="96725-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="96725-130">failedCount</span></span>|<span data-ttu-id="96725-131">Int32</span><span class="sxs-lookup"><span data-stu-id="96725-131">Int32</span></span>|<span data-ttu-id="96725-132">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="96725-132">Number of failed users</span></span>|
|<span data-ttu-id="96725-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="96725-133">notApplicableCount</span></span>|<span data-ttu-id="96725-134">Int32</span><span class="sxs-lookup"><span data-stu-id="96725-134">Int32</span></span>|<span data-ttu-id="96725-135">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="96725-135">Number of not applicable users</span></span>|
|<span data-ttu-id="96725-136">successCount</span><span class="sxs-lookup"><span data-stu-id="96725-136">successCount</span></span>|<span data-ttu-id="96725-137">Int32</span><span class="sxs-lookup"><span data-stu-id="96725-137">Int32</span></span>|<span data-ttu-id="96725-138">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="96725-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="96725-139">関係</span><span class="sxs-lookup"><span data-stu-id="96725-139">Relationships</span></span>
<span data-ttu-id="96725-140">なし</span><span class="sxs-lookup"><span data-stu-id="96725-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96725-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96725-141">JSON Representation</span></span>
<span data-ttu-id="96725-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96725-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```




