---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリケーションのプロビジョニングの構成をグループに割り当てるためのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6996bf29776910d8af3da08d63003889b817cfbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912135"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="010f3-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="010f3-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="010f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="010f3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="010f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="010f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="010f3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="010f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="010f3-107">アプリケーションのプロビジョニングの構成をグループに割り当てるためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="010f3-107">Contains the properties used to assign an App provisioning configuration to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="010f3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="010f3-108">Methods</span></span>
|<span data-ttu-id="010f3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="010f3-109">Method</span></span>|<span data-ttu-id="010f3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="010f3-110">Return Type</span></span>|<span data-ttu-id="010f3-111">説明</span><span class="sxs-lookup"><span data-stu-id="010f3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="010f3-112">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="010f3-112">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="010f3-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="010f3-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="010f3-114">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="010f3-114">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="010f3-115">MobileAppProvisioningConfigGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="010f3-115">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="010f3-116">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="010f3-116">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="010f3-117">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="010f3-117">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="010f3-118">MobileAppProvisioningConfigGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="010f3-118">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="010f3-119">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="010f3-119">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="010f3-120">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="010f3-120">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="010f3-121">MobileAppProvisioningConfigGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="010f3-121">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="010f3-122">なし</span><span class="sxs-lookup"><span data-stu-id="010f3-122">None</span></span>|<span data-ttu-id="010f3-123">の[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="010f3-123">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="010f3-124">MobileAppProvisioningConfigGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="010f3-124">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="010f3-125">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="010f3-125">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="010f3-126">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="010f3-126">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="010f3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="010f3-127">Properties</span></span>
|<span data-ttu-id="010f3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="010f3-128">Property</span></span>|<span data-ttu-id="010f3-129">型</span><span class="sxs-lookup"><span data-stu-id="010f3-129">Type</span></span>|<span data-ttu-id="010f3-130">説明</span><span class="sxs-lookup"><span data-stu-id="010f3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="010f3-131">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="010f3-131">targetGroupId</span></span>|<span data-ttu-id="010f3-132">String</span><span class="sxs-lookup"><span data-stu-id="010f3-132">String</span></span>|<span data-ttu-id="010f3-133">構成のプロビジョニング、アプリケーションが対象である AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="010f3-133">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="010f3-134">id</span><span class="sxs-lookup"><span data-stu-id="010f3-134">id</span></span>|<span data-ttu-id="010f3-135">String</span><span class="sxs-lookup"><span data-stu-id="010f3-135">String</span></span>|<span data-ttu-id="010f3-136">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="010f3-136">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="010f3-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="010f3-137">Relationships</span></span>
<span data-ttu-id="010f3-138">なし</span><span class="sxs-lookup"><span data-stu-id="010f3-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="010f3-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="010f3-139">JSON Representation</span></span>
<span data-ttu-id="010f3-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="010f3-140">Here is a JSON representation of the resource.</span></span>
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





