---
title: managedDeviceMobileAppConfigurationAssignment リソースの種類
description: グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c04947c63a72ebb1476ce5c863731a876987d603
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830178"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="11b37-103">managedDeviceMobileAppConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11b37-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="11b37-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11b37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11b37-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11b37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11b37-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="11b37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11b37-107">グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="11b37-107">Contains the properties used to assign an MDM app configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="11b37-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="11b37-108">Methods</span></span>
|<span data-ttu-id="11b37-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="11b37-109">Method</span></span>|<span data-ttu-id="11b37-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="11b37-110">Return Type</span></span>|<span data-ttu-id="11b37-111">説明</span><span class="sxs-lookup"><span data-stu-id="11b37-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11b37-112">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="11b37-112">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="11b37-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="11b37-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11b37-114">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="11b37-114">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="11b37-115">managedDeviceMobileAppConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="11b37-115">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="11b37-116">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="11b37-116">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="11b37-117">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="11b37-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="11b37-118">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="11b37-118">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="11b37-119">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="11b37-119">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="11b37-120">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="11b37-120">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="11b37-121">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="11b37-121">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="11b37-122">なし</span><span class="sxs-lookup"><span data-stu-id="11b37-122">None</span></span>|<span data-ttu-id="11b37-123">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="11b37-123">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="11b37-124">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="11b37-124">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="11b37-125">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="11b37-125">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="11b37-126">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="11b37-126">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11b37-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11b37-127">Properties</span></span>
|<span data-ttu-id="11b37-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11b37-128">Property</span></span>|<span data-ttu-id="11b37-129">種類</span><span class="sxs-lookup"><span data-stu-id="11b37-129">Type</span></span>|<span data-ttu-id="11b37-130">説明</span><span class="sxs-lookup"><span data-stu-id="11b37-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b37-131">ID</span><span class="sxs-lookup"><span data-stu-id="11b37-131">id</span></span>|<span data-ttu-id="11b37-132">String</span><span class="sxs-lookup"><span data-stu-id="11b37-132">String</span></span>|<span data-ttu-id="11b37-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="11b37-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="11b37-134">target</span><span class="sxs-lookup"><span data-stu-id="11b37-134">target</span></span>|[<span data-ttu-id="11b37-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="11b37-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="11b37-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="11b37-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11b37-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="11b37-137">Relationships</span></span>
<span data-ttu-id="11b37-138">なし</span><span class="sxs-lookup"><span data-stu-id="11b37-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11b37-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11b37-139">JSON Representation</span></span>
<span data-ttu-id="11b37-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="11b37-140">Here is a JSON representation of the resource.</span></span>
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





