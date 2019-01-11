---
title: embeddedSIMActivationCodePoolAssignment リソースの種類
description: 埋め込み SIM アクティベーション コード プール割り当てエンティティには、AAD のデバイス ・ グループに特定の embeddedSIMActivationCodePool が割り当てられます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8faac932014d4dc770748daa6a3d883b4e648d70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843310"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a><span data-ttu-id="3ea68-103">embeddedSIMActivationCodePoolAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ea68-103">embeddedSIMActivationCodePoolAssignment resource type</span></span>

> <span data-ttu-id="3ea68-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ea68-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ea68-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ea68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ea68-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ea68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ea68-107">埋め込み SIM アクティベーション コード プール割り当てエンティティには、AAD のデバイス ・ グループに特定の embeddedSIMActivationCodePool が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="3ea68-107">The embedded SIM activation code pool assignment entity assigns a specific embeddedSIMActivationCodePool to an AAD device group.</span></span>
## <a name="methods"></a><span data-ttu-id="3ea68-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ea68-108">Methods</span></span>
|<span data-ttu-id="3ea68-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3ea68-109">Method</span></span>|<span data-ttu-id="3ea68-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3ea68-110">Return Type</span></span>|<span data-ttu-id="3ea68-111">説明</span><span class="sxs-lookup"><span data-stu-id="3ea68-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3ea68-112">リスト embeddedSIMActivationCodePoolAssignments</span><span class="sxs-lookup"><span data-stu-id="3ea68-112">List embeddedSIMActivationCodePoolAssignments</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|<span data-ttu-id="3ea68-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3ea68-113">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) collection</span></span>|<span data-ttu-id="3ea68-114">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-114">List properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) objects.</span></span>|
|[<span data-ttu-id="3ea68-115">EmbeddedSIMActivationCodePoolAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-115">Get embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[<span data-ttu-id="3ea68-116">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="3ea68-116">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="3ea68-117">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ea68-117">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="3ea68-118">EmbeddedSIMActivationCodePoolAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-118">Create embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[<span data-ttu-id="3ea68-119">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="3ea68-119">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="3ea68-120">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-120">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|
|[<span data-ttu-id="3ea68-121">EmbeddedSIMActivationCodePoolAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-121">Delete embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|<span data-ttu-id="3ea68-122">なし</span><span class="sxs-lookup"><span data-stu-id="3ea68-122">None</span></span>|<span data-ttu-id="3ea68-123">の[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-123">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>|
|[<span data-ttu-id="3ea68-124">EmbeddedSIMActivationCodePoolAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-124">Update embeddedSIMActivationCodePoolAssignment</span></span>](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[<span data-ttu-id="3ea68-125">embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="3ea68-125">embeddedSIMActivationCodePoolAssignment</span></span>](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|<span data-ttu-id="3ea68-126">[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3ea68-126">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ea68-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ea68-127">Properties</span></span>
|<span data-ttu-id="3ea68-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ea68-128">Property</span></span>|<span data-ttu-id="3ea68-129">種類</span><span class="sxs-lookup"><span data-stu-id="3ea68-129">Type</span></span>|<span data-ttu-id="3ea68-130">説明</span><span class="sxs-lookup"><span data-stu-id="3ea68-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea68-131">ID</span><span class="sxs-lookup"><span data-stu-id="3ea68-131">id</span></span>|<span data-ttu-id="3ea68-132">String</span><span class="sxs-lookup"><span data-stu-id="3ea68-132">String</span></span>|<span data-ttu-id="3ea68-133">埋め込み SIM アクティベーション コードのプール割り当ての一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="3ea68-133">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="3ea68-134">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3ea68-134">System generated value assigned when created.</span></span>|
|<span data-ttu-id="3ea68-135">ターゲット</span><span class="sxs-lookup"><span data-stu-id="3ea68-135">target</span></span>|[<span data-ttu-id="3ea68-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3ea68-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3ea68-137">SIM のアクティブ化コードの埋め込み、プールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="3ea68-137">The type of groups targeted by the embedded SIM activation code pool.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ea68-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ea68-138">Relationships</span></span>
<span data-ttu-id="3ea68-139">なし</span><span class="sxs-lookup"><span data-stu-id="3ea68-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ea68-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ea68-140">JSON Representation</span></span>
<span data-ttu-id="3ea68-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ea68-141">Here is a JSON representation of the resource.</span></span>
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





