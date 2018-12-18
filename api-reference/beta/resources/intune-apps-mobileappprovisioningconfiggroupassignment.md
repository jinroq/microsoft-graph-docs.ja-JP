---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリケーションのプロビジョニングの構成をグループに割り当てるためのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: c38faf3f8de9aea79667664051bba6e45c83c238
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356484"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="7a70f-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a70f-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="7a70f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a70f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a70f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a70f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a70f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a70f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a70f-107">アプリケーションのプロビジョニングの構成をグループに割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a70f-107">Contains the properties used to assign an App provisioning configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="7a70f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a70f-108">Methods</span></span>
|<span data-ttu-id="7a70f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a70f-109">Method</span></span>|<span data-ttu-id="7a70f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a70f-110">Return Type</span></span>|<span data-ttu-id="7a70f-111">説明</span><span class="sxs-lookup"><span data-stu-id="7a70f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a70f-112">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="7a70f-112">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="7a70f-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7a70f-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="7a70f-114">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-114">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="7a70f-115">MobileAppProvisioningConfigGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-115">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="7a70f-116">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a70f-116">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="7a70f-117">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a70f-117">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="7a70f-118">MobileAppProvisioningConfigGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-118">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="7a70f-119">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a70f-119">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="7a70f-120">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-120">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="7a70f-121">MobileAppProvisioningConfigGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-121">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="7a70f-122">なし</span><span class="sxs-lookup"><span data-stu-id="7a70f-122">None</span></span>|<span data-ttu-id="7a70f-123">の[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-123">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="7a70f-124">MobileAppProvisioningConfigGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-124">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="7a70f-125">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7a70f-125">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="7a70f-126">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7a70f-126">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a70f-127">Properties</span><span class="sxs-lookup"><span data-stu-id="7a70f-127">Properties</span></span>
|<span data-ttu-id="7a70f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a70f-128">Property</span></span>|<span data-ttu-id="7a70f-129">種類</span><span class="sxs-lookup"><span data-stu-id="7a70f-129">Type</span></span>|<span data-ttu-id="7a70f-130">説明</span><span class="sxs-lookup"><span data-stu-id="7a70f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a70f-131">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="7a70f-131">targetGroupId</span></span>|<span data-ttu-id="7a70f-132">String</span><span class="sxs-lookup"><span data-stu-id="7a70f-132">String</span></span>|<span data-ttu-id="7a70f-133">構成のプロビジョニング、アプリケーションが対象である AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="7a70f-133">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="7a70f-134">id</span><span class="sxs-lookup"><span data-stu-id="7a70f-134">id</span></span>|<span data-ttu-id="7a70f-135">String</span><span class="sxs-lookup"><span data-stu-id="7a70f-135">String</span></span>|<span data-ttu-id="7a70f-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7a70f-136">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a70f-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a70f-137">Relationships</span></span>
<span data-ttu-id="7a70f-138">なし</span><span class="sxs-lookup"><span data-stu-id="7a70f-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a70f-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a70f-139">JSON Representation</span></span>
<span data-ttu-id="7a70f-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a70f-140">Here is a JSON representation of the resource.</span></span>
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





