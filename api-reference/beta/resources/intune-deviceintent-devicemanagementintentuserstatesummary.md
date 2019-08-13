---
title: deviceManagementIntentUserStateSummary リソースの種類
description: 目的のユーザー状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c934dd2035b628b8424a75c0b95a2e642c67586c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364755"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="090dd-103">deviceManagementIntentUserStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="090dd-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="090dd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="090dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="090dd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="090dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="090dd-106">目的のユーザー状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="090dd-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="090dd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="090dd-107">Methods</span></span>
|<span data-ttu-id="090dd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="090dd-108">Method</span></span>|<span data-ttu-id="090dd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="090dd-109">Return Type</span></span>|<span data-ttu-id="090dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="090dd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="090dd-111">DeviceManagementIntentUserStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="090dd-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="090dd-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="090dd-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="090dd-113">[DeviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="090dd-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="090dd-114">DeviceManagementIntentUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="090dd-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="090dd-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="090dd-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="090dd-116">[DeviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="090dd-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="090dd-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="090dd-117">Properties</span></span>
|<span data-ttu-id="090dd-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="090dd-118">Property</span></span>|<span data-ttu-id="090dd-119">型</span><span class="sxs-lookup"><span data-stu-id="090dd-119">Type</span></span>|<span data-ttu-id="090dd-120">説明</span><span class="sxs-lookup"><span data-stu-id="090dd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="090dd-121">id</span><span class="sxs-lookup"><span data-stu-id="090dd-121">id</span></span>|<span data-ttu-id="090dd-122">String</span><span class="sxs-lookup"><span data-stu-id="090dd-122">String</span></span>|<span data-ttu-id="090dd-123">ID</span><span class="sxs-lookup"><span data-stu-id="090dd-123">The ID</span></span>|
|<span data-ttu-id="090dd-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="090dd-124">conflictCount</span></span>|<span data-ttu-id="090dd-125">Int32</span><span class="sxs-lookup"><span data-stu-id="090dd-125">Int32</span></span>|<span data-ttu-id="090dd-126">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="090dd-126">Number of users in conflict</span></span>|
|<span data-ttu-id="090dd-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="090dd-127">errorCount</span></span>|<span data-ttu-id="090dd-128">Int32</span><span class="sxs-lookup"><span data-stu-id="090dd-128">Int32</span></span>|<span data-ttu-id="090dd-129">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="090dd-129">Number of error users</span></span>|
|<span data-ttu-id="090dd-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="090dd-130">failedCount</span></span>|<span data-ttu-id="090dd-131">Int32</span><span class="sxs-lookup"><span data-stu-id="090dd-131">Int32</span></span>|<span data-ttu-id="090dd-132">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="090dd-132">Number of failed users</span></span>|
|<span data-ttu-id="090dd-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="090dd-133">notApplicableCount</span></span>|<span data-ttu-id="090dd-134">Int32</span><span class="sxs-lookup"><span data-stu-id="090dd-134">Int32</span></span>|<span data-ttu-id="090dd-135">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="090dd-135">Number of not applicable users</span></span>|
|<span data-ttu-id="090dd-136">successCount</span><span class="sxs-lookup"><span data-stu-id="090dd-136">successCount</span></span>|<span data-ttu-id="090dd-137">Int32</span><span class="sxs-lookup"><span data-stu-id="090dd-137">Int32</span></span>|<span data-ttu-id="090dd-138">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="090dd-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="090dd-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="090dd-139">Relationships</span></span>
<span data-ttu-id="090dd-140">なし</span><span class="sxs-lookup"><span data-stu-id="090dd-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="090dd-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="090dd-141">JSON Representation</span></span>
<span data-ttu-id="090dd-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="090dd-142">Here is a JSON representation of the resource.</span></span>
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



