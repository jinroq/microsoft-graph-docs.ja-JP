---
title: mobileAppAssignment リソース タイプ
description: モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec9901c8f07e2ae56500c1b99aac1fcce1bfb379
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404520"
---
# <a name="mobileappassignment-resource-type"></a><span data-ttu-id="a7e0e-103">mobileAppAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a7e0e-103">mobileAppAssignment resource type</span></span>

> <span data-ttu-id="a7e0e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7e0e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7e0e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e0e-107">モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-107">A class containing the properties used for Group Assignment of a Mobile App.</span></span>

## <a name="methods"></a><span data-ttu-id="a7e0e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7e0e-108">Methods</span></span>
|<span data-ttu-id="a7e0e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7e0e-109">Method</span></span>|<span data-ttu-id="a7e0e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7e0e-110">Return Type</span></span>|<span data-ttu-id="a7e0e-111">説明</span><span class="sxs-lookup"><span data-stu-id="a7e0e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7e0e-112">List mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="a7e0e-112">List mobileAppAssignments</span></span>](../api/intune-apps-mobileappassignment-list.md)|<span data-ttu-id="a7e0e-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7e0e-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="a7e0e-114">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-114">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>|
|[<span data-ttu-id="a7e0e-115">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-115">Get mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-get.md)|[<span data-ttu-id="a7e0e-116">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-116">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="a7e0e-117">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-117">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="a7e0e-118">Create mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-118">Create mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-create.md)|[<span data-ttu-id="a7e0e-119">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-119">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="a7e0e-120">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-120">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="a7e0e-121">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-121">Delete mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-delete.md)|<span data-ttu-id="a7e0e-122">なし</span><span class="sxs-lookup"><span data-stu-id="a7e0e-122">None</span></span>|<span data-ttu-id="a7e0e-123">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-123">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>|
|[<span data-ttu-id="a7e0e-124">Update mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-124">Update mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-update.md)|[<span data-ttu-id="a7e0e-125">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7e0e-125">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="a7e0e-126">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-126">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7e0e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7e0e-127">Properties</span></span>
|<span data-ttu-id="a7e0e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7e0e-128">Property</span></span>|<span data-ttu-id="a7e0e-129">型</span><span class="sxs-lookup"><span data-stu-id="a7e0e-129">Type</span></span>|<span data-ttu-id="a7e0e-130">説明</span><span class="sxs-lookup"><span data-stu-id="a7e0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e0e-131">id</span><span class="sxs-lookup"><span data-stu-id="a7e0e-131">id</span></span>|<span data-ttu-id="a7e0e-132">String</span><span class="sxs-lookup"><span data-stu-id="a7e0e-132">String</span></span>|<span data-ttu-id="a7e0e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-133">Key of the entity.</span></span>|
|<span data-ttu-id="a7e0e-134">intent</span><span class="sxs-lookup"><span data-stu-id="a7e0e-134">intent</span></span>|[<span data-ttu-id="a7e0e-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="a7e0e-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a7e0e-136">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="a7e0e-137">target</span><span class="sxs-lookup"><span data-stu-id="a7e0e-137">target</span></span>|[<span data-ttu-id="a7e0e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a7e0e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a7e0e-139">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="a7e0e-140">settings</span><span class="sxs-lookup"><span data-stu-id="a7e0e-140">settings</span></span>|[<span data-ttu-id="a7e0e-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a7e0e-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="a7e0e-142">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-142">The settings for target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7e0e-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7e0e-143">Relationships</span></span>
<span data-ttu-id="a7e0e-144">なし</span><span class="sxs-lookup"><span data-stu-id="a7e0e-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7e0e-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7e0e-145">JSON Representation</span></span>
<span data-ttu-id="a7e0e-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7e0e-146">Here is a JSON representation of the resource.</span></span>
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




