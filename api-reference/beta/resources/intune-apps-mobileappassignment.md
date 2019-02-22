---
title: mobileAppAssignment リソース タイプ
description: モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77816742d4e7d736cad2941c3a49f2f6350ebd84
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140636"
---
# <a name="mobileappassignment-resource-type"></a><span data-ttu-id="77b1d-103">mobileAppAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="77b1d-103">mobileAppAssignment resource type</span></span>

> <span data-ttu-id="77b1d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77b1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77b1d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77b1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77b1d-106">モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。</span><span class="sxs-lookup"><span data-stu-id="77b1d-106">A class containing the properties used for Group Assignment of a Mobile App.</span></span>

## <a name="methods"></a><span data-ttu-id="77b1d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="77b1d-107">Methods</span></span>
|<span data-ttu-id="77b1d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="77b1d-108">Method</span></span>|<span data-ttu-id="77b1d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="77b1d-109">Return Type</span></span>|<span data-ttu-id="77b1d-110">説明</span><span class="sxs-lookup"><span data-stu-id="77b1d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="77b1d-111">List mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="77b1d-111">List mobileAppAssignments</span></span>](../api/intune-apps-mobileappassignment-list.md)|<span data-ttu-id="77b1d-112">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="77b1d-112">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="77b1d-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="77b1d-113">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>|
|[<span data-ttu-id="77b1d-114">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-114">Get mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-get.md)|[<span data-ttu-id="77b1d-115">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-115">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="77b1d-116">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="77b1d-116">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="77b1d-117">Create mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-117">Create mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-create.md)|[<span data-ttu-id="77b1d-118">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-118">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="77b1d-119">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="77b1d-119">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="77b1d-120">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-120">Delete mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-delete.md)|<span data-ttu-id="77b1d-121">なし</span><span class="sxs-lookup"><span data-stu-id="77b1d-121">None</span></span>|<span data-ttu-id="77b1d-122">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="77b1d-122">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>|
|[<span data-ttu-id="77b1d-123">Update mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-123">Update mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-update.md)|[<span data-ttu-id="77b1d-124">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="77b1d-124">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="77b1d-125">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="77b1d-125">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="77b1d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77b1d-126">Properties</span></span>
|<span data-ttu-id="77b1d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77b1d-127">Property</span></span>|<span data-ttu-id="77b1d-128">型</span><span class="sxs-lookup"><span data-stu-id="77b1d-128">Type</span></span>|<span data-ttu-id="77b1d-129">説明</span><span class="sxs-lookup"><span data-stu-id="77b1d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77b1d-130">id</span><span class="sxs-lookup"><span data-stu-id="77b1d-130">id</span></span>|<span data-ttu-id="77b1d-131">String</span><span class="sxs-lookup"><span data-stu-id="77b1d-131">String</span></span>|<span data-ttu-id="77b1d-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="77b1d-132">Key of the entity.</span></span>|
|<span data-ttu-id="77b1d-133">intent</span><span class="sxs-lookup"><span data-stu-id="77b1d-133">intent</span></span>|[<span data-ttu-id="77b1d-134">installIntent</span><span class="sxs-lookup"><span data-stu-id="77b1d-134">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="77b1d-135">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="77b1d-135">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="77b1d-136">target</span><span class="sxs-lookup"><span data-stu-id="77b1d-136">target</span></span>|[<span data-ttu-id="77b1d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="77b1d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="77b1d-138">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="77b1d-138">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="77b1d-139">settings</span><span class="sxs-lookup"><span data-stu-id="77b1d-139">settings</span></span>|[<span data-ttu-id="77b1d-140">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="77b1d-140">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="77b1d-141">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="77b1d-141">The settings for target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77b1d-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="77b1d-142">Relationships</span></span>
<span data-ttu-id="77b1d-143">なし</span><span class="sxs-lookup"><span data-stu-id="77b1d-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77b1d-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77b1d-144">JSON Representation</span></span>
<span data-ttu-id="77b1d-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="77b1d-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```




