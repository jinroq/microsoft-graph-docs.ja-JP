---
title: mobileAppAssignment リソース タイプ
description: モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。
ms.openlocfilehash: f6a84e40ccbdc2192e0d5f81d20d3d598f50f913
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067619"
---
# <a name="mobileappassignment-resource-type"></a><span data-ttu-id="dea93-103">mobileAppAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="dea93-103">mobileAppAssignment resource type</span></span>

> <span data-ttu-id="dea93-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dea93-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dea93-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dea93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dea93-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dea93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dea93-107">モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。</span><span class="sxs-lookup"><span data-stu-id="dea93-107">A class containing the properties used for Group Assignment of a Mobile App.</span></span>
## <a name="methods"></a><span data-ttu-id="dea93-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dea93-108">Methods</span></span>
|<span data-ttu-id="dea93-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dea93-109">Method</span></span>|<span data-ttu-id="dea93-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dea93-110">Return Type</span></span>|<span data-ttu-id="dea93-111">説明</span><span class="sxs-lookup"><span data-stu-id="dea93-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dea93-112">List mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="dea93-112">List mobileAppAssignments</span></span>](../api/intune-apps-mobileappassignment-list.md)|<span data-ttu-id="dea93-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dea93-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="dea93-114">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dea93-114">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>|
|[<span data-ttu-id="dea93-115">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-115">Get mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-get.md)|[<span data-ttu-id="dea93-116">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-116">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="dea93-117">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dea93-117">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="dea93-118">Create mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-118">Create mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-create.md)|[<span data-ttu-id="dea93-119">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-119">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="dea93-120">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dea93-120">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="dea93-121">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-121">Delete mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-delete.md)|<span data-ttu-id="dea93-122">なし</span><span class="sxs-lookup"><span data-stu-id="dea93-122">None</span></span>|<span data-ttu-id="dea93-123">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="dea93-123">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>|
|[<span data-ttu-id="dea93-124">Update mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-124">Update mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-update.md)|[<span data-ttu-id="dea93-125">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="dea93-125">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="dea93-126">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dea93-126">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dea93-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dea93-127">Properties</span></span>
|<span data-ttu-id="dea93-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dea93-128">Property</span></span>|<span data-ttu-id="dea93-129">型</span><span class="sxs-lookup"><span data-stu-id="dea93-129">Type</span></span>|<span data-ttu-id="dea93-130">説明</span><span class="sxs-lookup"><span data-stu-id="dea93-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea93-131">id</span><span class="sxs-lookup"><span data-stu-id="dea93-131">id</span></span>|<span data-ttu-id="dea93-132">String</span><span class="sxs-lookup"><span data-stu-id="dea93-132">String</span></span>|<span data-ttu-id="dea93-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dea93-133">Key of the entity.</span></span>|
|<span data-ttu-id="dea93-134">intent</span><span class="sxs-lookup"><span data-stu-id="dea93-134">intent</span></span>|[<span data-ttu-id="dea93-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="dea93-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="dea93-136">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="dea93-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="dea93-137">target</span><span class="sxs-lookup"><span data-stu-id="dea93-137">target</span></span>|[<span data-ttu-id="dea93-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dea93-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dea93-139">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="dea93-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="dea93-140">settings</span><span class="sxs-lookup"><span data-stu-id="dea93-140">settings</span></span>|[<span data-ttu-id="dea93-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="dea93-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="dea93-142">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="dea93-142">The settings for target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dea93-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dea93-143">Relationships</span></span>
<span data-ttu-id="dea93-144">なし</span><span class="sxs-lookup"><span data-stu-id="dea93-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dea93-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dea93-145">JSON Representation</span></span>
<span data-ttu-id="dea93-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dea93-146">Here is a JSON representation of the resource.</span></span>
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





