---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6af0d2547e5e63ed887e31983046944630f8cdf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772210"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a><span data-ttu-id="0f3a4-103">mobileAppProvisioningConfigGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f3a4-103">mobileAppProvisioningConfigGroupAssignment resource type</span></span>

> <span data-ttu-id="0f3a4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f3a4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f3a4-106">アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-106">Contains the properties used to assign an App provisioning configuration to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="0f3a4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f3a4-107">Methods</span></span>
|<span data-ttu-id="0f3a4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f3a4-108">Method</span></span>|<span data-ttu-id="0f3a4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0f3a4-109">Return Type</span></span>|<span data-ttu-id="0f3a4-110">説明</span><span class="sxs-lookup"><span data-stu-id="0f3a4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f3a4-111">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="0f3a4-111">List mobileAppProvisioningConfigGroupAssignments</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|<span data-ttu-id="0f3a4-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0f3a4-112">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="0f3a4-113">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-113">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="0f3a4-114">mobileAppProvisioningConfigGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="0f3a4-114">Get mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[<span data-ttu-id="0f3a4-115">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0f3a4-115">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="0f3a4-116">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-116">Read properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="0f3a4-117">mobileAppProvisioningConfigGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="0f3a4-117">Create mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[<span data-ttu-id="0f3a4-118">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0f3a4-118">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="0f3a4-119">新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-119">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|
|[<span data-ttu-id="0f3a4-120">mobileAppProvisioningConfigGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="0f3a4-120">Delete mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|<span data-ttu-id="0f3a4-121">なし</span><span class="sxs-lookup"><span data-stu-id="0f3a4-121">None</span></span>|<span data-ttu-id="0f3a4-122">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-122">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>|
|[<span data-ttu-id="0f3a4-123">mobileAppProvisioningConfigGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="0f3a4-123">Update mobileAppProvisioningConfigGroupAssignment</span></span>](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[<span data-ttu-id="0f3a4-124">mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0f3a4-124">mobileAppProvisioningConfigGroupAssignment</span></span>](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|<span data-ttu-id="0f3a4-125">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-125">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f3a4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f3a4-126">Properties</span></span>
|<span data-ttu-id="0f3a4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f3a4-127">Property</span></span>|<span data-ttu-id="0f3a4-128">型</span><span class="sxs-lookup"><span data-stu-id="0f3a4-128">Type</span></span>|<span data-ttu-id="0f3a4-129">説明</span><span class="sxs-lookup"><span data-stu-id="0f3a4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f3a4-130">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="0f3a4-130">targetGroupId</span></span>|<span data-ttu-id="0f3a4-131">文字列</span><span class="sxs-lookup"><span data-stu-id="0f3a4-131">String</span></span>|<span data-ttu-id="0f3a4-132">アプリのプロビジョニング構成を対象とする AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-132">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="0f3a4-133">id</span><span class="sxs-lookup"><span data-stu-id="0f3a4-133">id</span></span>|<span data-ttu-id="0f3a4-134">String</span><span class="sxs-lookup"><span data-stu-id="0f3a4-134">String</span></span>|<span data-ttu-id="0f3a4-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-135">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3a4-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f3a4-136">Relationships</span></span>
<span data-ttu-id="0f3a4-137">なし</span><span class="sxs-lookup"><span data-stu-id="0f3a4-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f3a4-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f3a4-138">JSON Representation</span></span>
<span data-ttu-id="0f3a4-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f3a4-139">Here is a JSON representation of the resource.</span></span>
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





