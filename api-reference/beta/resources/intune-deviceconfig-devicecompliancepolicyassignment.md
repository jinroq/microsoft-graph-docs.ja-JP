---
title: deviceCompliancePolicyAssignment リソースの種類
description: デバイス コンプライアンス ポリシーの割り当てです。
author: tfitzmac
ms.openlocfilehash: 9e589cb6191a7d8ca7406125419bcfae03304ade
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310676"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a><span data-ttu-id="b731c-103">deviceCompliancePolicyAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b731c-103">deviceCompliancePolicyAssignment resource type</span></span>

> <span data-ttu-id="b731c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b731c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b731c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b731c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b731c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b731c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b731c-107">デバイス コンプライアンス ポリシーの割り当てです。</span><span class="sxs-lookup"><span data-stu-id="b731c-107">Device compliance policy assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="b731c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b731c-108">Methods</span></span>
|<span data-ttu-id="b731c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b731c-109">Method</span></span>|<span data-ttu-id="b731c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b731c-110">Return Type</span></span>|<span data-ttu-id="b731c-111">説明</span><span class="sxs-lookup"><span data-stu-id="b731c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b731c-112">deviceCompliancePolicyAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="b731c-112">List deviceCompliancePolicyAssignments</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|<span data-ttu-id="b731c-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b731c-113">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="b731c-114">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b731c-114">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="b731c-115">deviceCompliancePolicyAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="b731c-115">Get deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[<span data-ttu-id="b731c-116">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b731c-116">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="b731c-117">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b731c-117">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="b731c-118">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="b731c-118">Create deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[<span data-ttu-id="b731c-119">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b731c-119">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="b731c-120">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b731c-120">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="b731c-121">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="b731c-121">Delete deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|<span data-ttu-id="b731c-122">なし</span><span class="sxs-lookup"><span data-stu-id="b731c-122">None</span></span>|<span data-ttu-id="b731c-123">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b731c-123">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>|
|[<span data-ttu-id="b731c-124">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="b731c-124">Update deviceCompliancePolicyAssignment</span></span>](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[<span data-ttu-id="b731c-125">deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b731c-125">deviceCompliancePolicyAssignment</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|<span data-ttu-id="b731c-126">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b731c-126">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b731c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b731c-127">Properties</span></span>
|<span data-ttu-id="b731c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b731c-128">Property</span></span>|<span data-ttu-id="b731c-129">種類</span><span class="sxs-lookup"><span data-stu-id="b731c-129">Type</span></span>|<span data-ttu-id="b731c-130">説明</span><span class="sxs-lookup"><span data-stu-id="b731c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b731c-131">ID</span><span class="sxs-lookup"><span data-stu-id="b731c-131">id</span></span>|<span data-ttu-id="b731c-132">String</span><span class="sxs-lookup"><span data-stu-id="b731c-132">String</span></span>|<span data-ttu-id="b731c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b731c-133">Key of the entity.</span></span>|
|<span data-ttu-id="b731c-134">target</span><span class="sxs-lookup"><span data-stu-id="b731c-134">target</span></span>|[<span data-ttu-id="b731c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b731c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b731c-136">デバイス コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="b731c-136">Target for the compliance policy assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b731c-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b731c-137">Relationships</span></span>
<span data-ttu-id="b731c-138">なし</span><span class="sxs-lookup"><span data-stu-id="b731c-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b731c-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b731c-139">JSON Representation</span></span>
<span data-ttu-id="b731c-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b731c-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




