---
title: mobileAppAssignment リソース タイプ
description: モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b418c6714db42f596ab8666cc7bd98eeddcb4c6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367396"
---
# <a name="mobileappassignment-resource-type"></a><span data-ttu-id="bb0ab-103">mobileAppAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="bb0ab-103">mobileAppAssignment resource type</span></span>

> <span data-ttu-id="bb0ab-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb0ab-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0ab-106">モバイル アプリのグループ割り当て用に使用されるプロパティを含むクラスです。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-106">A class containing the properties used for Group Assignment of a Mobile App.</span></span>

## <a name="methods"></a><span data-ttu-id="bb0ab-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb0ab-107">Methods</span></span>
|<span data-ttu-id="bb0ab-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb0ab-108">Method</span></span>|<span data-ttu-id="bb0ab-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb0ab-109">Return Type</span></span>|<span data-ttu-id="bb0ab-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb0ab-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb0ab-111">List mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="bb0ab-111">List mobileAppAssignments</span></span>](../api/intune-apps-mobileappassignment-list.md)|<span data-ttu-id="bb0ab-112">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bb0ab-112">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="bb0ab-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-113">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>|
|[<span data-ttu-id="bb0ab-114">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-114">Get mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-get.md)|[<span data-ttu-id="bb0ab-115">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-115">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="bb0ab-116">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-116">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="bb0ab-117">Create mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-117">Create mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-create.md)|[<span data-ttu-id="bb0ab-118">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-118">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="bb0ab-119">新しい [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-119">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="bb0ab-120">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-120">Delete mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-delete.md)|<span data-ttu-id="bb0ab-121">なし</span><span class="sxs-lookup"><span data-stu-id="bb0ab-121">None</span></span>|<span data-ttu-id="bb0ab-122">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-122">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>|
|[<span data-ttu-id="bb0ab-123">Update mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-123">Update mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-update.md)|[<span data-ttu-id="bb0ab-124">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="bb0ab-124">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="bb0ab-125">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-125">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb0ab-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb0ab-126">Properties</span></span>
|<span data-ttu-id="bb0ab-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb0ab-127">Property</span></span>|<span data-ttu-id="bb0ab-128">型</span><span class="sxs-lookup"><span data-stu-id="bb0ab-128">Type</span></span>|<span data-ttu-id="bb0ab-129">説明</span><span class="sxs-lookup"><span data-stu-id="bb0ab-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0ab-130">id</span><span class="sxs-lookup"><span data-stu-id="bb0ab-130">id</span></span>|<span data-ttu-id="bb0ab-131">String</span><span class="sxs-lookup"><span data-stu-id="bb0ab-131">String</span></span>|<span data-ttu-id="bb0ab-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-132">Key of the entity.</span></span>|
|<span data-ttu-id="bb0ab-133">intent</span><span class="sxs-lookup"><span data-stu-id="bb0ab-133">intent</span></span>|[<span data-ttu-id="bb0ab-134">installIntent</span><span class="sxs-lookup"><span data-stu-id="bb0ab-134">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="bb0ab-135">管理者によって定義されたインストールの目的。可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-135">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="bb0ab-136">target</span><span class="sxs-lookup"><span data-stu-id="bb0ab-136">target</span></span>|[<span data-ttu-id="bb0ab-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bb0ab-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bb0ab-138">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-138">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="bb0ab-139">settings</span><span class="sxs-lookup"><span data-stu-id="bb0ab-139">settings</span></span>|[<span data-ttu-id="bb0ab-140">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="bb0ab-140">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="bb0ab-141">管理者によって定義された、ターゲットの割り当ての設定。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-141">The settings for target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb0ab-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb0ab-142">Relationships</span></span>
<span data-ttu-id="bb0ab-143">なし</span><span class="sxs-lookup"><span data-stu-id="bb0ab-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb0ab-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb0ab-144">JSON Representation</span></span>
<span data-ttu-id="bb0ab-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb0ab-145">Here is a JSON representation of the resource.</span></span>
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



