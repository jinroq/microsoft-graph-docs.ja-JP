---
title: enrollmentConfigurationAssignment リソースの種類
description: 登録の構成の割り当て
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ed753720116456f11d67e9adbbb998222ed7191
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371349"
---
# <a name="enrollmentconfigurationassignment-resource-type"></a><span data-ttu-id="6ca1d-103">enrollmentConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ca1d-103">enrollmentConfigurationAssignment resource type</span></span>

> <span data-ttu-id="6ca1d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ca1d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ca1d-106">登録の構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="6ca1d-106">Enrollment Configuration Assignment</span></span>

## <a name="methods"></a><span data-ttu-id="6ca1d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ca1d-107">Methods</span></span>
|<span data-ttu-id="6ca1d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ca1d-108">Method</span></span>|<span data-ttu-id="6ca1d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6ca1d-109">Return Type</span></span>|<span data-ttu-id="6ca1d-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ca1d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ca1d-111">List enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="6ca1d-111">List enrollmentConfigurationAssignments</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-list.md)|<span data-ttu-id="6ca1d-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6ca1d-112">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6ca1d-113">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-113">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="6ca1d-114">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-114">Get enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-get.md)|[<span data-ttu-id="6ca1d-115">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-115">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="6ca1d-116">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-116">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6ca1d-117">Create enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-117">Create enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-create.md)|[<span data-ttu-id="6ca1d-118">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-118">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="6ca1d-119">新しい [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-119">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="6ca1d-120">Delete enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-120">Delete enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-delete.md)|<span data-ttu-id="6ca1d-121">なし</span><span class="sxs-lookup"><span data-stu-id="6ca1d-121">None</span></span>|<span data-ttu-id="6ca1d-122">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-122">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="6ca1d-123">Update enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-123">Update enrollmentConfigurationAssignment</span></span>](../api/intune-onboarding-enrollmentconfigurationassignment-update.md)|[<span data-ttu-id="6ca1d-124">enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ca1d-124">enrollmentConfigurationAssignment</span></span>](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|<span data-ttu-id="6ca1d-125">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-125">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ca1d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ca1d-126">Properties</span></span>
|<span data-ttu-id="6ca1d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ca1d-127">Property</span></span>|<span data-ttu-id="6ca1d-128">型</span><span class="sxs-lookup"><span data-stu-id="6ca1d-128">Type</span></span>|<span data-ttu-id="6ca1d-129">説明</span><span class="sxs-lookup"><span data-stu-id="6ca1d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ca1d-130">id</span><span class="sxs-lookup"><span data-stu-id="6ca1d-130">id</span></span>|<span data-ttu-id="6ca1d-131">String</span><span class="sxs-lookup"><span data-stu-id="6ca1d-131">String</span></span>|<span data-ttu-id="6ca1d-132">登録構成の割り当てのキー</span><span class="sxs-lookup"><span data-stu-id="6ca1d-132">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="6ca1d-133">target</span><span class="sxs-lookup"><span data-stu-id="6ca1d-133">target</span></span>|[<span data-ttu-id="6ca1d-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6ca1d-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6ca1d-135">テナント内の管理されたデバイスへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-135">Represents an assignment to managed devices in the tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ca1d-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ca1d-136">Relationships</span></span>
<span data-ttu-id="6ca1d-137">なし</span><span class="sxs-lookup"><span data-stu-id="6ca1d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ca1d-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ca1d-138">JSON Representation</span></span>
<span data-ttu-id="6ca1d-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ca1d-139">Here is a JSON representation of the resource.</span></span>
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



