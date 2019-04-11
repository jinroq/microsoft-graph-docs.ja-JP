---
title: deviceConfigurationUserStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d6d79f4e36ae66aa871f08eaa69aaa2bcf39a76
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779371"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a><span data-ttu-id="98703-103">deviceConfigurationUserStateSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98703-103">deviceConfigurationUserStateSummary resource type</span></span>

> <span data-ttu-id="98703-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98703-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98703-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="98703-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98703-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="98703-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="98703-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="98703-107">Methods</span></span>
|<span data-ttu-id="98703-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="98703-108">Method</span></span>|<span data-ttu-id="98703-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="98703-109">Return Type</span></span>|<span data-ttu-id="98703-110">説明</span><span class="sxs-lookup"><span data-stu-id="98703-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="98703-111">deviceConfigurationUserStateSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="98703-111">Get deviceConfigurationUserStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[<span data-ttu-id="98703-112">deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="98703-112">deviceConfigurationUserStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|<span data-ttu-id="98703-113">[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="98703-113">Read properties and relationships of the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="98703-114">deviceConfigurationUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="98703-114">Update deviceConfigurationUserStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[<span data-ttu-id="98703-115">deviceConfigurationUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="98703-115">deviceConfigurationUserStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|<span data-ttu-id="98703-116">[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="98703-116">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98703-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98703-117">Properties</span></span>
|<span data-ttu-id="98703-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98703-118">Property</span></span>|<span data-ttu-id="98703-119">型</span><span class="sxs-lookup"><span data-stu-id="98703-119">Type</span></span>|<span data-ttu-id="98703-120">説明</span><span class="sxs-lookup"><span data-stu-id="98703-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98703-121">id</span><span class="sxs-lookup"><span data-stu-id="98703-121">id</span></span>|<span data-ttu-id="98703-122">String</span><span class="sxs-lookup"><span data-stu-id="98703-122">String</span></span>|<span data-ttu-id="98703-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="98703-123">Key of the entity.</span></span>|
|<span data-ttu-id="98703-124">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-124">unknownUserCount</span></span>|<span data-ttu-id="98703-125">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-125">Int32</span></span>|<span data-ttu-id="98703-126">不明なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-126">Number of unknown users</span></span>|
|<span data-ttu-id="98703-127">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-127">notApplicableUserCount</span></span>|<span data-ttu-id="98703-128">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-128">Int32</span></span>|<span data-ttu-id="98703-129">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-129">Number of not applicable users</span></span>|
|<span data-ttu-id="98703-130">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-130">compliantUserCount</span></span>|<span data-ttu-id="98703-131">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-131">Int32</span></span>|<span data-ttu-id="98703-132">準拠しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-132">Number of compliant users</span></span>|
|<span data-ttu-id="98703-133">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-133">remediatedUserCount</span></span>|<span data-ttu-id="98703-134">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-134">Int32</span></span>|<span data-ttu-id="98703-135">修復したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-135">Number of remediated users</span></span>|
|<span data-ttu-id="98703-136">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-136">nonCompliantUserCount</span></span>|<span data-ttu-id="98703-137">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-137">Int32</span></span>|<span data-ttu-id="98703-138">準拠していないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-138">Number of NonCompliant users</span></span>|
|<span data-ttu-id="98703-139">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-139">errorUserCount</span></span>|<span data-ttu-id="98703-140">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-140">Int32</span></span>|<span data-ttu-id="98703-141">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-141">Number of error users</span></span>|
|<span data-ttu-id="98703-142">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="98703-142">conflictUserCount</span></span>|<span data-ttu-id="98703-143">Int32</span><span class="sxs-lookup"><span data-stu-id="98703-143">Int32</span></span>|<span data-ttu-id="98703-144">競合ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="98703-144">Number of conflict users</span></span>|

## <a name="relationships"></a><span data-ttu-id="98703-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98703-145">Relationships</span></span>
<span data-ttu-id="98703-146">なし</span><span class="sxs-lookup"><span data-stu-id="98703-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98703-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98703-147">JSON Representation</span></span>
<span data-ttu-id="98703-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98703-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```





