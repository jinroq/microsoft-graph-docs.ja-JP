---
title: managedEBookAssignment リソースの種類
description: グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6d6cdc1cbe5b2eb7b734219dbb7c67152afe3a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423546"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="9050f-103">managedEBookAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9050f-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="9050f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9050f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9050f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9050f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9050f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9050f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9050f-107">グループへの電子ブックの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9050f-107">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="9050f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9050f-108">Methods</span></span>
|<span data-ttu-id="9050f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="9050f-109">Method</span></span>|<span data-ttu-id="9050f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9050f-110">Return Type</span></span>|<span data-ttu-id="9050f-111">説明</span><span class="sxs-lookup"><span data-stu-id="9050f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9050f-112">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="9050f-112">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="9050f-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9050f-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="9050f-114">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9050f-114">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="9050f-115">managedEBookAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="9050f-115">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="9050f-116">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9050f-116">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="9050f-117">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9050f-117">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="9050f-118">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="9050f-118">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="9050f-119">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9050f-119">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="9050f-120">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9050f-120">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="9050f-121">managedEBookAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="9050f-121">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="9050f-122">なし</span><span class="sxs-lookup"><span data-stu-id="9050f-122">None</span></span>|<span data-ttu-id="9050f-123">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="9050f-123">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="9050f-124">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="9050f-124">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="9050f-125">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9050f-125">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="9050f-126">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9050f-126">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9050f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9050f-127">Properties</span></span>
|<span data-ttu-id="9050f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9050f-128">Property</span></span>|<span data-ttu-id="9050f-129">型</span><span class="sxs-lookup"><span data-stu-id="9050f-129">Type</span></span>|<span data-ttu-id="9050f-130">説明</span><span class="sxs-lookup"><span data-stu-id="9050f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9050f-131">id</span><span class="sxs-lookup"><span data-stu-id="9050f-131">id</span></span>|<span data-ttu-id="9050f-132">String</span><span class="sxs-lookup"><span data-stu-id="9050f-132">String</span></span>|<span data-ttu-id="9050f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9050f-133">Key of the entity.</span></span>|
|<span data-ttu-id="9050f-134">target</span><span class="sxs-lookup"><span data-stu-id="9050f-134">target</span></span>|[<span data-ttu-id="9050f-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9050f-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9050f-136">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="9050f-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="9050f-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="9050f-137">installIntent</span></span>|[<span data-ttu-id="9050f-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="9050f-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="9050f-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="9050f-139">The install intent for eBook.</span></span> <span data-ttu-id="9050f-140">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="9050f-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9050f-141">関係</span><span class="sxs-lookup"><span data-stu-id="9050f-141">Relationships</span></span>
<span data-ttu-id="9050f-142">なし</span><span class="sxs-lookup"><span data-stu-id="9050f-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9050f-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9050f-143">JSON Representation</span></span>
<span data-ttu-id="9050f-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9050f-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```




