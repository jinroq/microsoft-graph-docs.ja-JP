---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 884ddf889b755aa174a93e07584d39ff1d2a8ddf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156239"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="0783c-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0783c-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="0783c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0783c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0783c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0783c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0783c-106">アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0783c-106">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="0783c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0783c-107">Methods</span></span>
|<span data-ttu-id="0783c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0783c-108">Method</span></span>|<span data-ttu-id="0783c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0783c-109">Return Type</span></span>|<span data-ttu-id="0783c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0783c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0783c-111">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="0783c-111">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="0783c-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0783c-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="0783c-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0783c-113">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="0783c-114">mobileAppProvisioningConfigGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="0783c-114">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="0783c-115">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0783c-115">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="0783c-116">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0783c-116">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="0783c-117">mobileAppProvisioningConfigGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="0783c-117">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="0783c-118">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0783c-118">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="0783c-119">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0783c-119">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="0783c-120">mobileAppProvisioningConfigGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="0783c-120">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="0783c-121">なし</span><span class="sxs-lookup"><span data-stu-id="0783c-121">None</span></span>|<span data-ttu-id="0783c-122">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0783c-122">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="0783c-123">mobileAppProvisioningConfigGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="0783c-123">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="0783c-124">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0783c-124">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="0783c-125">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0783c-125">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0783c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0783c-126">Properties</span></span>
|<span data-ttu-id="0783c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0783c-127">Property</span></span>|<span data-ttu-id="0783c-128">型</span><span class="sxs-lookup"><span data-stu-id="0783c-128">Type</span></span>|<span data-ttu-id="0783c-129">説明</span><span class="sxs-lookup"><span data-stu-id="0783c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0783c-130">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="0783c-130">targetGroupId</span></span>|<span data-ttu-id="0783c-131">String</span><span class="sxs-lookup"><span data-stu-id="0783c-131">String</span></span>|<span data-ttu-id="0783c-132">アプリのプロビジョニング構成を対象とする AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="0783c-132">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="0783c-133">id</span><span class="sxs-lookup"><span data-stu-id="0783c-133">id</span></span>|<span data-ttu-id="0783c-134">String</span><span class="sxs-lookup"><span data-stu-id="0783c-134">String</span></span>|<span data-ttu-id="0783c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0783c-135">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0783c-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0783c-136">Relationships</span></span>
<span data-ttu-id="0783c-137">なし</span><span class="sxs-lookup"><span data-stu-id="0783c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0783c-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0783c-138">JSON Representation</span></span>
<span data-ttu-id="0783c-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0783c-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppProvisioningConfigGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "String",
  "id": "String (identifier)"
}
```




