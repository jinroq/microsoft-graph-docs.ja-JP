---
title: managedDeviceMobileAppConfigurationAssignment リソースの種類
description: グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99d7c1deef4733b492596928dde8500581e8f5eb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250538"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="ece52-103">managedDeviceMobileAppConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ece52-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="ece52-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ece52-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece52-105">グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ece52-105">Contains the properties used to assign an MDM app configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="ece52-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ece52-106">Methods</span></span>
|<span data-ttu-id="ece52-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ece52-107">Method</span></span>|<span data-ttu-id="ece52-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ece52-108">Return Type</span></span>|<span data-ttu-id="ece52-109">説明</span><span class="sxs-lookup"><span data-stu-id="ece52-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ece52-110">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="ece52-110">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="ece52-111">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ece52-111">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ece52-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ece52-112">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="ece52-113">managedDeviceMobileAppConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="ece52-113">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="ece52-114">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ece52-114">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="ece52-115">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ece52-115">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="ece52-116">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ece52-116">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="ece52-117">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ece52-117">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="ece52-118">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ece52-118">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="ece52-119">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="ece52-119">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="ece52-120">なし</span><span class="sxs-lookup"><span data-stu-id="ece52-120">None</span></span>|<span data-ttu-id="ece52-121">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ece52-121">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="ece52-122">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="ece52-122">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="ece52-123">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ece52-123">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="ece52-124">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ece52-124">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ece52-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ece52-125">Properties</span></span>
|<span data-ttu-id="ece52-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ece52-126">Property</span></span>|<span data-ttu-id="ece52-127">型</span><span class="sxs-lookup"><span data-stu-id="ece52-127">Type</span></span>|<span data-ttu-id="ece52-128">説明</span><span class="sxs-lookup"><span data-stu-id="ece52-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ece52-129">id</span><span class="sxs-lookup"><span data-stu-id="ece52-129">id</span></span>|<span data-ttu-id="ece52-130">String</span><span class="sxs-lookup"><span data-stu-id="ece52-130">String</span></span>|<span data-ttu-id="ece52-131">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ece52-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ece52-132">target</span><span class="sxs-lookup"><span data-stu-id="ece52-132">target</span></span>|[<span data-ttu-id="ece52-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ece52-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ece52-134">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="ece52-134">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ece52-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ece52-135">Relationships</span></span>
<span data-ttu-id="ece52-136">なし</span><span class="sxs-lookup"><span data-stu-id="ece52-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ece52-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ece52-137">JSON Representation</span></span>
<span data-ttu-id="ece52-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ece52-138">Here is a JSON representation of the resource.</span></span>
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



