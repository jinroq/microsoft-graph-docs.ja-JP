---
title: devicemanagementintentassignment リソースの種類
description: インテント割り当てエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a955187e079e1f77accb21361bfe49689f52108
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522427"
---
# <a name="devicemanagementintentassignment-resource-type"></a><span data-ttu-id="e13a5-103">devicemanagementintentassignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e13a5-103">deviceManagementIntentAssignment resource type</span></span>

> <span data-ttu-id="e13a5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e13a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e13a5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e13a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e13a5-106">インテント割り当てエンティティ</span><span class="sxs-lookup"><span data-stu-id="e13a5-106">Intent assignment entity</span></span>

## <a name="methods"></a><span data-ttu-id="e13a5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e13a5-107">Methods</span></span>
|<span data-ttu-id="e13a5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e13a5-108">Method</span></span>|<span data-ttu-id="e13a5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e13a5-109">Return Type</span></span>|<span data-ttu-id="e13a5-110">説明</span><span class="sxs-lookup"><span data-stu-id="e13a5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e13a5-111">devicemanagementintentassignments のリスト</span><span class="sxs-lookup"><span data-stu-id="e13a5-111">List deviceManagementIntentAssignments</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|<span data-ttu-id="e13a5-112">[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e13a5-112">[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) collection</span></span>|<span data-ttu-id="e13a5-113">[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e13a5-113">List properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) objects.</span></span>|
|[<span data-ttu-id="e13a5-114">devicemanagementintentassignment の取得</span><span class="sxs-lookup"><span data-stu-id="e13a5-114">Get deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[<span data-ttu-id="e13a5-115">devicemanagementintentassignment</span><span class="sxs-lookup"><span data-stu-id="e13a5-115">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="e13a5-116">[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e13a5-116">Read properties and relationships of the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="e13a5-117">devicemanagementintentassignment の作成</span><span class="sxs-lookup"><span data-stu-id="e13a5-117">Create deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[<span data-ttu-id="e13a5-118">devicemanagementintentassignment</span><span class="sxs-lookup"><span data-stu-id="e13a5-118">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="e13a5-119">新しい[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e13a5-119">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|
|[<span data-ttu-id="e13a5-120">devicemanagementintentassignment の削除</span><span class="sxs-lookup"><span data-stu-id="e13a5-120">Delete deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|<span data-ttu-id="e13a5-121">なし</span><span class="sxs-lookup"><span data-stu-id="e13a5-121">None</span></span>|<span data-ttu-id="e13a5-122">[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e13a5-122">Deletes a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>|
|[<span data-ttu-id="e13a5-123">devicemanagementintentassignment の更新</span><span class="sxs-lookup"><span data-stu-id="e13a5-123">Update deviceManagementIntentAssignment</span></span>](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[<span data-ttu-id="e13a5-124">devicemanagementintentassignment</span><span class="sxs-lookup"><span data-stu-id="e13a5-124">deviceManagementIntentAssignment</span></span>](../resources/intune-deviceintent-devicemanagementintentassignment.md)|<span data-ttu-id="e13a5-125">[devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e13a5-125">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e13a5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e13a5-126">Properties</span></span>
|<span data-ttu-id="e13a5-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e13a5-127">Property</span></span>|<span data-ttu-id="e13a5-128">型</span><span class="sxs-lookup"><span data-stu-id="e13a5-128">Type</span></span>|<span data-ttu-id="e13a5-129">説明</span><span class="sxs-lookup"><span data-stu-id="e13a5-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e13a5-130">id</span><span class="sxs-lookup"><span data-stu-id="e13a5-130">id</span></span>|<span data-ttu-id="e13a5-131">String</span><span class="sxs-lookup"><span data-stu-id="e13a5-131">String</span></span>|<span data-ttu-id="e13a5-132">割り当て ID</span><span class="sxs-lookup"><span data-stu-id="e13a5-132">The assignment ID</span></span>|
|<span data-ttu-id="e13a5-133">target</span><span class="sxs-lookup"><span data-stu-id="e13a5-133">target</span></span>|[<span data-ttu-id="e13a5-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e13a5-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e13a5-135">割り当て先</span><span class="sxs-lookup"><span data-stu-id="e13a5-135">The assignment target</span></span>|

## <a name="relationships"></a><span data-ttu-id="e13a5-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e13a5-136">Relationships</span></span>
<span data-ttu-id="e13a5-137">なし</span><span class="sxs-lookup"><span data-stu-id="e13a5-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e13a5-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e13a5-138">JSON Representation</span></span>
<span data-ttu-id="e13a5-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e13a5-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```







