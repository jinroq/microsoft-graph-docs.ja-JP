---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60b92a7b1232ba19a4166171fa118b18f7a263b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163393"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="660dd-103">embeddedSIMActivationCodePoolAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="660dd-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="660dd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="660dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="660dd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="660dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="660dd-106">埋め込まれた SIM ライセンス認証コードプール割り当てエンティティは、特定の embeddedSIMActivationCodePool を AAD デバイスグループに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="660dd-106">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="660dd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="660dd-107">Methods</span></span>
|<span data-ttu-id="660dd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="660dd-108">Method</span></span>|<span data-ttu-id="660dd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="660dd-109">Return Type</span></span>|<span data-ttu-id="660dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="660dd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="660dd-111">リスト embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="660dd-111">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="660dd-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="660dd-112">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="660dd-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="660dd-113">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="660dd-114">embeddedSIMActivationCodePoolAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="660dd-114">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="660dd-115">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="660dd-115">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="660dd-116">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="660dd-116">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="660dd-117">embeddedSIMActivationCodePoolAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="660dd-117">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="660dd-118">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="660dd-118">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="660dd-119">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="660dd-119">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="660dd-120">embeddedSIMActivationCodePoolAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="660dd-120">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="660dd-121">なし</span><span class="sxs-lookup"><span data-stu-id="660dd-121">None</span></span>|<span data-ttu-id="660dd-122">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="660dd-122">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="660dd-123">embeddedSIMActivationCodePoolAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="660dd-123">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="660dd-124">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="660dd-124">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="660dd-125">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="660dd-125">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="660dd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="660dd-126">Properties</span></span>
|<span data-ttu-id="660dd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="660dd-127">Property</span></span>|<span data-ttu-id="660dd-128">型</span><span class="sxs-lookup"><span data-stu-id="660dd-128">Type</span></span>|<span data-ttu-id="660dd-129">説明</span><span class="sxs-lookup"><span data-stu-id="660dd-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="660dd-130">id</span><span class="sxs-lookup"><span data-stu-id="660dd-130">id</span></span>|<span data-ttu-id="660dd-131">String</span><span class="sxs-lookup"><span data-stu-id="660dd-131">String</span></span>|<span data-ttu-id="660dd-132">埋め込まれている SIM ライセンス認証コードプールの割り当ての一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="660dd-132">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="660dd-133">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="660dd-133">System generated value assigned when created.</span></span>|
|<span data-ttu-id="660dd-134">target</span><span class="sxs-lookup"><span data-stu-id="660dd-134">target</span></span>|[<span data-ttu-id="660dd-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="660dd-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="660dd-136">埋め込まれた SIM アクティブ化コードプールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="660dd-136">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="660dd-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="660dd-137">Relationships</span></span>
<span data-ttu-id="660dd-138">なし</span><span class="sxs-lookup"><span data-stu-id="660dd-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="660dd-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="660dd-139">JSON Representation</span></span>
<span data-ttu-id="660dd-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="660dd-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




