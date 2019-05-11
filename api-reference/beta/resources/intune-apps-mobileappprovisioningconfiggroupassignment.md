---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c01dfd8da7d241719ca873fa910338a286f16dbd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949914"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="29c0c-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29c0c-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="29c0c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29c0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29c0c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29c0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29c0c-106">アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="29c0c-106">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="29c0c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="29c0c-107">Methods</span></span>
|<span data-ttu-id="29c0c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="29c0c-108">Method</span></span>|<span data-ttu-id="29c0c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29c0c-109">Return Type</span></span>|<span data-ttu-id="29c0c-110">説明</span><span class="sxs-lookup"><span data-stu-id="29c0c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29c0c-111">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="29c0c-111">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="29c0c-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29c0c-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="29c0c-113">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="29c0c-113">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="29c0c-114">MobileAppProvisioningConfigGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="29c0c-114">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="29c0c-115">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="29c0c-115">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="29c0c-116">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="29c0c-116">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="29c0c-117">MobileAppProvisioningConfigGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="29c0c-117">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="29c0c-118">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="29c0c-118">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="29c0c-119">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="29c0c-119">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="29c0c-120">MobileAppProvisioningConfigGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="29c0c-120">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="29c0c-121">None</span><span class="sxs-lookup"><span data-stu-id="29c0c-121">None</span></span>|<span data-ttu-id="29c0c-122">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="29c0c-122">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="29c0c-123">MobileAppProvisioningConfigGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="29c0c-123">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="29c0c-124">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="29c0c-124">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="29c0c-125">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29c0c-125">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29c0c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29c0c-126">Properties</span></span>
|<span data-ttu-id="29c0c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29c0c-127">Property</span></span>|<span data-ttu-id="29c0c-128">型</span><span class="sxs-lookup"><span data-stu-id="29c0c-128">Type</span></span>|<span data-ttu-id="29c0c-129">説明</span><span class="sxs-lookup"><span data-stu-id="29c0c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29c0c-130">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="29c0c-130">targetGroupId</span></span>|<span data-ttu-id="29c0c-131">String</span><span class="sxs-lookup"><span data-stu-id="29c0c-131">String</span></span>|<span data-ttu-id="29c0c-132">アプリのプロビジョニング構成を対象とする AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="29c0c-132">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="29c0c-133">id</span><span class="sxs-lookup"><span data-stu-id="29c0c-133">id</span></span>|<span data-ttu-id="29c0c-134">String</span><span class="sxs-lookup"><span data-stu-id="29c0c-134">String</span></span>|<span data-ttu-id="29c0c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29c0c-135">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29c0c-136">関係</span><span class="sxs-lookup"><span data-stu-id="29c0c-136">Relationships</span></span>
<span data-ttu-id="29c0c-137">なし</span><span class="sxs-lookup"><span data-stu-id="29c0c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29c0c-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29c0c-138">JSON Representation</span></span>
<span data-ttu-id="29c0c-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29c0c-139">Here is a JSON representation of the resource.</span></span>
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




