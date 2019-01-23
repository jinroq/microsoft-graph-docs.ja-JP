---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリケーションのプロビジョニングの構成をグループに割り当てるためのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ad07112031ce8ebe46d48c2c5fa51f0744a2bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421929"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="b379d-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b379d-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="b379d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b379d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b379d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b379d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b379d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b379d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b379d-107">アプリケーションのプロビジョニングの構成をグループに割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b379d-107">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="b379d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b379d-108">Methods</span></span>
|<span data-ttu-id="b379d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b379d-109">Method</span></span>|<span data-ttu-id="b379d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b379d-110">Return Type</span></span>|<span data-ttu-id="b379d-111">説明</span><span class="sxs-lookup"><span data-stu-id="b379d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b379d-112">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="b379d-112">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="b379d-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b379d-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="b379d-114">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b379d-114">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="b379d-115">MobileAppProvisioningConfigGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="b379d-115">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="b379d-116">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b379d-116">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="b379d-117">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b379d-117">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="b379d-118">MobileAppProvisioningConfigGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="b379d-118">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="b379d-119">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b379d-119">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="b379d-120">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b379d-120">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="b379d-121">MobileAppProvisioningConfigGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="b379d-121">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="b379d-122">なし</span><span class="sxs-lookup"><span data-stu-id="b379d-122">None</span></span>|<span data-ttu-id="b379d-123">の[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b379d-123">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="b379d-124">MobileAppProvisioningConfigGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="b379d-124">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="b379d-125">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b379d-125">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="b379d-126">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b379d-126">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b379d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b379d-127">Properties</span></span>
|<span data-ttu-id="b379d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b379d-128">Property</span></span>|<span data-ttu-id="b379d-129">型</span><span class="sxs-lookup"><span data-stu-id="b379d-129">Type</span></span>|<span data-ttu-id="b379d-130">説明</span><span class="sxs-lookup"><span data-stu-id="b379d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b379d-131">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="b379d-131">targetGroupId</span></span>|<span data-ttu-id="b379d-132">String</span><span class="sxs-lookup"><span data-stu-id="b379d-132">String</span></span>|<span data-ttu-id="b379d-133">構成のプロビジョニング、アプリケーションが対象である AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="b379d-133">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="b379d-134">id</span><span class="sxs-lookup"><span data-stu-id="b379d-134">id</span></span>|<span data-ttu-id="b379d-135">String</span><span class="sxs-lookup"><span data-stu-id="b379d-135">String</span></span>|<span data-ttu-id="b379d-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b379d-136">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b379d-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b379d-137">Relationships</span></span>
<span data-ttu-id="b379d-138">なし</span><span class="sxs-lookup"><span data-stu-id="b379d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b379d-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b379d-139">JSON Representation</span></span>
<span data-ttu-id="b379d-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b379d-140">Here is a JSON representation of the resource.</span></span>
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




