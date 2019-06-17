---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3883c8e088a57a0709f47deea1c3210049dab301
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991836"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="a63bf-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a63bf-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="a63bf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a63bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a63bf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a63bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a63bf-106">アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a63bf-106">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="a63bf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a63bf-107">Methods</span></span>
|<span data-ttu-id="a63bf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a63bf-108">Method</span></span>|<span data-ttu-id="a63bf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a63bf-109">Return Type</span></span>|<span data-ttu-id="a63bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="a63bf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a63bf-111">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="a63bf-111">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="a63bf-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a63bf-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="a63bf-113">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a63bf-113">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="a63bf-114">MobileAppProvisioningConfigGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="a63bf-114">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="a63bf-115">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a63bf-115">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="a63bf-116">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a63bf-116">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="a63bf-117">MobileAppProvisioningConfigGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="a63bf-117">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="a63bf-118">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a63bf-118">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="a63bf-119">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a63bf-119">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="a63bf-120">MobileAppProvisioningConfigGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="a63bf-120">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="a63bf-121">None</span><span class="sxs-lookup"><span data-stu-id="a63bf-121">None</span></span>|<span data-ttu-id="a63bf-122">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="a63bf-122">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="a63bf-123">MobileAppProvisioningConfigGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="a63bf-123">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="a63bf-124">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a63bf-124">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="a63bf-125">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a63bf-125">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a63bf-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a63bf-126">Properties</span></span>
|<span data-ttu-id="a63bf-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a63bf-127">Property</span></span>|<span data-ttu-id="a63bf-128">型</span><span class="sxs-lookup"><span data-stu-id="a63bf-128">Type</span></span>|<span data-ttu-id="a63bf-129">説明</span><span class="sxs-lookup"><span data-stu-id="a63bf-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a63bf-130">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="a63bf-130">targetGroupId</span></span>|<span data-ttu-id="a63bf-131">String</span><span class="sxs-lookup"><span data-stu-id="a63bf-131">String</span></span>|<span data-ttu-id="a63bf-132">アプリのプロビジョニング構成を対象とする AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="a63bf-132">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="a63bf-133">id</span><span class="sxs-lookup"><span data-stu-id="a63bf-133">id</span></span>|<span data-ttu-id="a63bf-134">String</span><span class="sxs-lookup"><span data-stu-id="a63bf-134">String</span></span>|<span data-ttu-id="a63bf-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a63bf-135">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a63bf-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a63bf-136">Relationships</span></span>
<span data-ttu-id="a63bf-137">なし</span><span class="sxs-lookup"><span data-stu-id="a63bf-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a63bf-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a63bf-138">JSON Representation</span></span>
<span data-ttu-id="a63bf-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a63bf-139">Here is a JSON representation of the resource.</span></span>
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





