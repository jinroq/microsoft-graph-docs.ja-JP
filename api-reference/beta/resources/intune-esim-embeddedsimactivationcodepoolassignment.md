---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込み SIM アクティベーション コード プール割り当てエンティティには、AAD のデバイス ・ グループに特定の embeddedSIMActivationCodePool が割り当てられます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ed8918adb99e301717ed7d53e54bb3ff1ac29ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423840"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="6c905-103">embeddedSIMActivationCodePoolAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c905-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="6c905-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c905-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c905-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c905-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c905-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c905-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c905-107">埋め込み SIM アクティベーション コード プール割り当てエンティティには、AAD のデバイス ・ グループに特定の embeddedSIMActivationCodePool が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="6c905-107">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>

## <a name="methods"></a><span data-ttu-id="6c905-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c905-108">Methods</span></span>
|<span data-ttu-id="6c905-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c905-109">Method</span></span>|<span data-ttu-id="6c905-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6c905-110">Return Type</span></span>|<span data-ttu-id="6c905-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c905-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c905-112">リスト embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="6c905-112">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="6c905-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6c905-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="6c905-114">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6c905-114">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="6c905-115">EmbeddedSIMActivationCodePoolAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c905-115">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="6c905-116">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="6c905-116">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="6c905-117">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c905-117">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="6c905-118">EmbeddedSIMActivationCodePoolAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="6c905-118">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="6c905-119">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="6c905-119">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="6c905-120">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6c905-120">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="6c905-121">EmbeddedSIMActivationCodePoolAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c905-121">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="6c905-122">なし</span><span class="sxs-lookup"><span data-stu-id="6c905-122">None</span></span>|<span data-ttu-id="6c905-123">の[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6c905-123">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="6c905-124">EmbeddedSIMActivationCodePoolAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="6c905-124">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="6c905-125">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="6c905-125">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="6c905-126">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c905-126">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c905-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c905-127">Properties</span></span>
|<span data-ttu-id="6c905-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c905-128">Property</span></span>|<span data-ttu-id="6c905-129">型</span><span class="sxs-lookup"><span data-stu-id="6c905-129">Type</span></span>|<span data-ttu-id="6c905-130">説明</span><span class="sxs-lookup"><span data-stu-id="6c905-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c905-131">id</span><span class="sxs-lookup"><span data-stu-id="6c905-131">id</span></span>|<span data-ttu-id="6c905-132">String</span><span class="sxs-lookup"><span data-stu-id="6c905-132">String</span></span>|<span data-ttu-id="6c905-133">埋め込み SIM アクティベーション コードのプール割り当ての一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6c905-133">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="6c905-134">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="6c905-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="6c905-135">target</span><span class="sxs-lookup"><span data-stu-id="6c905-135">target</span></span>|[<span data-ttu-id="6c905-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6c905-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6c905-137">SIM のアクティブ化コードの埋め込み、プールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="6c905-137">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c905-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c905-138">Relationships</span></span>
<span data-ttu-id="6c905-139">なし</span><span class="sxs-lookup"><span data-stu-id="6c905-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c905-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c905-140">JSON Representation</span></span>
<span data-ttu-id="6c905-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c905-141">Here is a JSON representation of the resource.</span></span>
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




