---
title: managedDeviceMobileAppConfigurationAssignment リソースの種類
description: グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 064f881f0d90d2748446bcd618b07767c4836db5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149981"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="0befd-103">managedDeviceMobileAppConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0befd-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="0befd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0befd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0befd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0befd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0befd-106">グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0befd-106">Contains the properties used to assign an MDM app configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="0befd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0befd-107">Methods</span></span>
|<span data-ttu-id="0befd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0befd-108">Method</span></span>|<span data-ttu-id="0befd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0befd-109">Return Type</span></span>|<span data-ttu-id="0befd-110">説明</span><span class="sxs-lookup"><span data-stu-id="0befd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0befd-111">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="0befd-111">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="0befd-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0befd-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0befd-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0befd-113">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="0befd-114">managedDeviceMobileAppConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="0befd-114">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="0befd-115">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0befd-115">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="0befd-116">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0befd-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="0befd-117">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="0befd-117">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="0befd-118">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0befd-118">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="0befd-119">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0befd-119">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="0befd-120">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="0befd-120">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="0befd-121">なし</span><span class="sxs-lookup"><span data-stu-id="0befd-121">None</span></span>|<span data-ttu-id="0befd-122">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0befd-122">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="0befd-123">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="0befd-123">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="0befd-124">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0befd-124">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="0befd-125">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0befd-125">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0befd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0befd-126">Properties</span></span>
|<span data-ttu-id="0befd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0befd-127">Property</span></span>|<span data-ttu-id="0befd-128">型</span><span class="sxs-lookup"><span data-stu-id="0befd-128">Type</span></span>|<span data-ttu-id="0befd-129">説明</span><span class="sxs-lookup"><span data-stu-id="0befd-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0befd-130">id</span><span class="sxs-lookup"><span data-stu-id="0befd-130">id</span></span>|<span data-ttu-id="0befd-131">String</span><span class="sxs-lookup"><span data-stu-id="0befd-131">String</span></span>|<span data-ttu-id="0befd-132">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0befd-132">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0befd-133">target</span><span class="sxs-lookup"><span data-stu-id="0befd-133">target</span></span>|[<span data-ttu-id="0befd-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0befd-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0befd-135">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="0befd-135">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0befd-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0befd-136">Relationships</span></span>
<span data-ttu-id="0befd-137">なし</span><span class="sxs-lookup"><span data-stu-id="0befd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0befd-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0befd-138">JSON Representation</span></span>
<span data-ttu-id="0befd-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0befd-139">Here is a JSON representation of the resource.</span></span>
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




