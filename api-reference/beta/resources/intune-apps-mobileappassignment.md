---
title: mobileAppAssignment リソース タイプ
description: モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cc7fae4134c4566d3530e7ec06ade57d03c6b352
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991364"
---
# <a name="mobileappassignment-resource-type"></a><span data-ttu-id="4fb29-103">mobileAppAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="4fb29-103">mobileAppAssignment resource type</span></span>

> <span data-ttu-id="4fb29-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fb29-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fb29-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fb29-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fb29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fb29-107">モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。</span><span class="sxs-lookup"><span data-stu-id="4fb29-107">A class containing the properties used for Group Assignment of a Mobile App.</span></span>
## <a name="methods"></a><span data-ttu-id="4fb29-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb29-108">Methods</span></span>
|<span data-ttu-id="4fb29-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb29-109">Method</span></span>|<span data-ttu-id="4fb29-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fb29-110">Return Type</span></span>|<span data-ttu-id="4fb29-111">説明</span><span class="sxs-lookup"><span data-stu-id="4fb29-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4fb29-112">List mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="4fb29-112">List mobileAppAssignments</span></span>](../api/intune-apps-mobileappassignment-list.md)|<span data-ttu-id="4fb29-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb29-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="4fb29-114">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4fb29-114">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>|
|[<span data-ttu-id="4fb29-115">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-115">Get mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-get.md)|[<span data-ttu-id="4fb29-116">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-116">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="4fb29-117">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4fb29-117">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="4fb29-118">Create mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-118">Create mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-create.md)|[<span data-ttu-id="4fb29-119">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-119">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="4fb29-120">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fb29-120">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="4fb29-121">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-121">Delete mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-delete.md)|<span data-ttu-id="4fb29-122">なし</span><span class="sxs-lookup"><span data-stu-id="4fb29-122">None</span></span>|<span data-ttu-id="4fb29-123">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4fb29-123">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>|
|[<span data-ttu-id="4fb29-124">Update mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-124">Update mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-update.md)|[<span data-ttu-id="4fb29-125">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4fb29-125">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="4fb29-126">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4fb29-126">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4fb29-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb29-127">Properties</span></span>
|<span data-ttu-id="4fb29-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb29-128">Property</span></span>|<span data-ttu-id="4fb29-129">種類</span><span class="sxs-lookup"><span data-stu-id="4fb29-129">Type</span></span>|<span data-ttu-id="4fb29-130">説明</span><span class="sxs-lookup"><span data-stu-id="4fb29-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb29-131">ID</span><span class="sxs-lookup"><span data-stu-id="4fb29-131">id</span></span>|<span data-ttu-id="4fb29-132">String</span><span class="sxs-lookup"><span data-stu-id="4fb29-132">String</span></span>|<span data-ttu-id="4fb29-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4fb29-133">Key of the entity.</span></span>|
|<span data-ttu-id="4fb29-134">intent</span><span class="sxs-lookup"><span data-stu-id="4fb29-134">intent</span></span>|[<span data-ttu-id="4fb29-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="4fb29-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="4fb29-136">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="4fb29-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="4fb29-137">target</span><span class="sxs-lookup"><span data-stu-id="4fb29-137">target</span></span>|[<span data-ttu-id="4fb29-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4fb29-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4fb29-139">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="4fb29-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="4fb29-140">settings</span><span class="sxs-lookup"><span data-stu-id="4fb29-140">settings</span></span>|[<span data-ttu-id="4fb29-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="4fb29-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="4fb29-142">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="4fb29-142">The settings for target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fb29-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fb29-143">Relationships</span></span>
<span data-ttu-id="4fb29-144">なし</span><span class="sxs-lookup"><span data-stu-id="4fb29-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4fb29-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fb29-145">JSON Representation</span></span>
<span data-ttu-id="4fb29-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fb29-146">Here is a JSON representation of the resource.</span></span>
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





