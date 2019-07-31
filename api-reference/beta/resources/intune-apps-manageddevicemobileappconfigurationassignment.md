---
title: managedDeviceMobileAppConfigurationAssignment リソースの種類
description: グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 928c9c84b5216ab1d0f75437b8aa2095ad01d793
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005311"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a><span data-ttu-id="2ec59-103">managedDeviceMobileAppConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ec59-103">managedDeviceMobileAppConfigurationAssignment resource type</span></span>

> <span data-ttu-id="2ec59-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ec59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ec59-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ec59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ec59-106">グループに MDM アプリ構成を割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ec59-106">Contains the properties used to assign an MDM app configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="2ec59-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ec59-107">Methods</span></span>
|<span data-ttu-id="2ec59-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ec59-108">Method</span></span>|<span data-ttu-id="2ec59-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ec59-109">Return Type</span></span>|<span data-ttu-id="2ec59-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ec59-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ec59-111">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="2ec59-111">List managedDeviceMobileAppConfigurationAssignments</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|<span data-ttu-id="2ec59-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ec59-112">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2ec59-113">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2ec59-113">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2ec59-114">managedDeviceMobileAppConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="2ec59-114">Get managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[<span data-ttu-id="2ec59-115">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ec59-115">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="2ec59-116">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ec59-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2ec59-117">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="2ec59-117">Create managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[<span data-ttu-id="2ec59-118">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ec59-118">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="2ec59-119">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2ec59-119">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2ec59-120">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="2ec59-120">Delete managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|<span data-ttu-id="2ec59-121">なし</span><span class="sxs-lookup"><span data-stu-id="2ec59-121">None</span></span>|<span data-ttu-id="2ec59-122">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="2ec59-122">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2ec59-123">managedDeviceMobileAppConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="2ec59-123">Update managedDeviceMobileAppConfigurationAssignment</span></span>](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[<span data-ttu-id="2ec59-124">managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ec59-124">managedDeviceMobileAppConfigurationAssignment</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|<span data-ttu-id="2ec59-125">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ec59-125">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ec59-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ec59-126">Properties</span></span>
|<span data-ttu-id="2ec59-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ec59-127">Property</span></span>|<span data-ttu-id="2ec59-128">型</span><span class="sxs-lookup"><span data-stu-id="2ec59-128">Type</span></span>|<span data-ttu-id="2ec59-129">説明</span><span class="sxs-lookup"><span data-stu-id="2ec59-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ec59-130">id</span><span class="sxs-lookup"><span data-stu-id="2ec59-130">id</span></span>|<span data-ttu-id="2ec59-131">String</span><span class="sxs-lookup"><span data-stu-id="2ec59-131">String</span></span>|<span data-ttu-id="2ec59-132">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2ec59-132">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2ec59-133">target</span><span class="sxs-lookup"><span data-stu-id="2ec59-133">target</span></span>|[<span data-ttu-id="2ec59-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2ec59-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2ec59-135">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="2ec59-135">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ec59-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ec59-136">Relationships</span></span>
<span data-ttu-id="2ec59-137">なし</span><span class="sxs-lookup"><span data-stu-id="2ec59-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ec59-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ec59-138">JSON Representation</span></span>
<span data-ttu-id="2ec59-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ec59-139">Here is a JSON representation of the resource.</span></span>
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





