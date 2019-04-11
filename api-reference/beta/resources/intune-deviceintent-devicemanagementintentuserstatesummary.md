---
title: deviceManagementIntentUserStateSummary リソースの種類
description: 目的のユーザー状態の概要を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 538d1e5da36a1d90aac95641175eb0cebeeb69c3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790012"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="a3cbf-103">deviceManagementIntentUserStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3cbf-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="a3cbf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3cbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3cbf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3cbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3cbf-106">目的のユーザー状態の概要を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="a3cbf-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="a3cbf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3cbf-107">Methods</span></span>
|<span data-ttu-id="a3cbf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3cbf-108">Method</span></span>|<span data-ttu-id="a3cbf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a3cbf-109">Return Type</span></span>|<span data-ttu-id="a3cbf-110">説明</span><span class="sxs-lookup"><span data-stu-id="a3cbf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3cbf-111">deviceManagementIntentUserStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="a3cbf-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="a3cbf-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="a3cbf-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="a3cbf-113">[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a3cbf-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="a3cbf-114">deviceManagementIntentUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a3cbf-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="a3cbf-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="a3cbf-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="a3cbf-116">[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3cbf-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3cbf-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3cbf-117">Properties</span></span>
|<span data-ttu-id="a3cbf-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3cbf-118">Property</span></span>|<span data-ttu-id="a3cbf-119">型</span><span class="sxs-lookup"><span data-stu-id="a3cbf-119">Type</span></span>|<span data-ttu-id="a3cbf-120">説明</span><span class="sxs-lookup"><span data-stu-id="a3cbf-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3cbf-121">id</span><span class="sxs-lookup"><span data-stu-id="a3cbf-121">id</span></span>|<span data-ttu-id="a3cbf-122">String</span><span class="sxs-lookup"><span data-stu-id="a3cbf-122">String</span></span>|<span data-ttu-id="a3cbf-123">ID</span><span class="sxs-lookup"><span data-stu-id="a3cbf-123">The ID</span></span>|
|<span data-ttu-id="a3cbf-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a3cbf-124">conflictCount</span></span>|<span data-ttu-id="a3cbf-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a3cbf-125">Int32</span></span>|<span data-ttu-id="a3cbf-126">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a3cbf-126">Number of users in conflict</span></span>|
|<span data-ttu-id="a3cbf-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="a3cbf-127">errorCount</span></span>|<span data-ttu-id="a3cbf-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a3cbf-128">Int32</span></span>|<span data-ttu-id="a3cbf-129">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a3cbf-129">Number of error users</span></span>|
|<span data-ttu-id="a3cbf-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="a3cbf-130">failedCount</span></span>|<span data-ttu-id="a3cbf-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a3cbf-131">Int32</span></span>|<span data-ttu-id="a3cbf-132">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a3cbf-132">Number of failed users</span></span>|
|<span data-ttu-id="a3cbf-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a3cbf-133">notApplicableCount</span></span>|<span data-ttu-id="a3cbf-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a3cbf-134">Int32</span></span>|<span data-ttu-id="a3cbf-135">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a3cbf-135">Number of not applicable users</span></span>|
|<span data-ttu-id="a3cbf-136">successCount</span><span class="sxs-lookup"><span data-stu-id="a3cbf-136">successCount</span></span>|<span data-ttu-id="a3cbf-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a3cbf-137">Int32</span></span>|<span data-ttu-id="a3cbf-138">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="a3cbf-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3cbf-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3cbf-139">Relationships</span></span>
<span data-ttu-id="a3cbf-140">なし</span><span class="sxs-lookup"><span data-stu-id="a3cbf-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3cbf-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3cbf-141">JSON Representation</span></span>
<span data-ttu-id="a3cbf-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3cbf-142">Here is a JSON representation of the resource.</span></span>
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





