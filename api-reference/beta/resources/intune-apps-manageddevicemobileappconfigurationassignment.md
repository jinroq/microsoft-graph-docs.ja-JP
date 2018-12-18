---
title: managedDeviceMobileAppConfigurationAssignment リソースの種類
description: グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 6e84c0a8624e868bc9fb1b76714c60f883375945
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312587"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="be3ca-103">managedDeviceMobileAppConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be3ca-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="be3ca-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be3ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be3ca-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be3ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be3ca-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be3ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be3ca-107">グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="be3ca-107">Contains the properties used to assign an MDM app configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="be3ca-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="be3ca-108">Methods</span></span>
|<span data-ttu-id="be3ca-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="be3ca-109">Method</span></span>|<span data-ttu-id="be3ca-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be3ca-110">Return Type</span></span>|<span data-ttu-id="be3ca-111">説明</span><span class="sxs-lookup"><span data-stu-id="be3ca-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be3ca-112">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="be3ca-112">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="be3ca-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be3ca-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="be3ca-114">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="be3ca-114">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="be3ca-115">managedDeviceMobileAppConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="be3ca-115">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="be3ca-116">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="be3ca-116">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="be3ca-117">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="be3ca-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="be3ca-118">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="be3ca-118">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="be3ca-119">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="be3ca-119">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="be3ca-120">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="be3ca-120">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="be3ca-121">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="be3ca-121">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="be3ca-122">なし</span><span class="sxs-lookup"><span data-stu-id="be3ca-122">None</span></span>|<span data-ttu-id="be3ca-123">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="be3ca-123">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="be3ca-124">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="be3ca-124">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="be3ca-125">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="be3ca-125">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="be3ca-126">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="be3ca-126">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="be3ca-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be3ca-127">Properties</span></span>
|<span data-ttu-id="be3ca-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be3ca-128">Property</span></span>|<span data-ttu-id="be3ca-129">種類</span><span class="sxs-lookup"><span data-stu-id="be3ca-129">Type</span></span>|<span data-ttu-id="be3ca-130">説明</span><span class="sxs-lookup"><span data-stu-id="be3ca-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be3ca-131">ID</span><span class="sxs-lookup"><span data-stu-id="be3ca-131">id</span></span>|<span data-ttu-id="be3ca-132">String</span><span class="sxs-lookup"><span data-stu-id="be3ca-132">String</span></span>|<span data-ttu-id="be3ca-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="be3ca-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="be3ca-134">target</span><span class="sxs-lookup"><span data-stu-id="be3ca-134">target</span></span>|[<span data-ttu-id="be3ca-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="be3ca-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="be3ca-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="be3ca-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be3ca-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be3ca-137">Relationships</span></span>
<span data-ttu-id="be3ca-138">なし</span><span class="sxs-lookup"><span data-stu-id="be3ca-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="be3ca-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be3ca-139">JSON Representation</span></span>
<span data-ttu-id="be3ca-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be3ca-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





