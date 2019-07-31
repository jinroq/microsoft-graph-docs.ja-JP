---
title: enrollmentConfigurationAssignment リソースの種類
description: 登録の構成の割り当て
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 130ab9bb56edbcce610f8d0f09a5cc05482bdf1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998024"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a><span data-ttu-id="43ed6-103">enrollmentConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43ed6-103">enrollmentConfigurationAssignment resource type</span></span>

> <span data-ttu-id="43ed6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43ed6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43ed6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43ed6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43ed6-106">登録の構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="43ed6-106">Enrollment Configuration Assignment</span></span>

## <a name="methods"></a><span data-ttu-id="43ed6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="43ed6-107">Methods</span></span>
|<span data-ttu-id="43ed6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="43ed6-108">Method</span></span>|<span data-ttu-id="43ed6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="43ed6-109">Return Type</span></span>|<span data-ttu-id="43ed6-110">説明</span><span class="sxs-lookup"><span data-stu-id="43ed6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43ed6-111">List enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="43ed6-111">List enrollmentConfigurationAssignments</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|<span data-ttu-id="43ed6-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="43ed6-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="43ed6-113">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="43ed6-113">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="43ed6-114">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-114">Get enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[<span data-ttu-id="43ed6-115">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-115">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="43ed6-116">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="43ed6-116">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="43ed6-117">Create enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-117">Create enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[<span data-ttu-id="43ed6-118">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-118">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="43ed6-119">新しい [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43ed6-119">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="43ed6-120">Delete enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-120">Delete enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|<span data-ttu-id="43ed6-121">なし</span><span class="sxs-lookup"><span data-stu-id="43ed6-121">None</span></span>|<span data-ttu-id="43ed6-122">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="43ed6-122">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="43ed6-123">Update enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-123">Update enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[<span data-ttu-id="43ed6-124">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="43ed6-124">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="43ed6-125">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="43ed6-125">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43ed6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43ed6-126">Properties</span></span>
|<span data-ttu-id="43ed6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43ed6-127">Property</span></span>|<span data-ttu-id="43ed6-128">型</span><span class="sxs-lookup"><span data-stu-id="43ed6-128">Type</span></span>|<span data-ttu-id="43ed6-129">説明</span><span class="sxs-lookup"><span data-stu-id="43ed6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43ed6-130">id</span><span class="sxs-lookup"><span data-stu-id="43ed6-130">id</span></span>|<span data-ttu-id="43ed6-131">String</span><span class="sxs-lookup"><span data-stu-id="43ed6-131">String</span></span>|<span data-ttu-id="43ed6-132">登録構成の割り当てのキー</span><span class="sxs-lookup"><span data-stu-id="43ed6-132">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="43ed6-133">target</span><span class="sxs-lookup"><span data-stu-id="43ed6-133">target</span></span>|[<span data-ttu-id="43ed6-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="43ed6-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="43ed6-135">テナント内の管理されたデバイスへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="43ed6-135">Represents an assignment to managed devices in the tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="43ed6-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43ed6-136">Relationships</span></span>
<span data-ttu-id="43ed6-137">なし</span><span class="sxs-lookup"><span data-stu-id="43ed6-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43ed6-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43ed6-138">JSON Representation</span></span>
<span data-ttu-id="43ed6-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43ed6-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





