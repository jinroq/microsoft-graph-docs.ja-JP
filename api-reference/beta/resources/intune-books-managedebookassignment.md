---
title: managedEBookAssignment リソースの種類
description: グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39fc5a56e4fb63a62a4fe2c15dd478efda426636
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949865"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="9829a-103">managedEBookAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9829a-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="9829a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9829a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9829a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9829a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9829a-106">グループへの電子ブックの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9829a-106">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="9829a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9829a-107">Methods</span></span>
|<span data-ttu-id="9829a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="9829a-108">Method</span></span>|<span data-ttu-id="9829a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9829a-109">Return Type</span></span>|<span data-ttu-id="9829a-110">説明</span><span class="sxs-lookup"><span data-stu-id="9829a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9829a-111">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="9829a-111">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="9829a-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9829a-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="9829a-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9829a-113">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="9829a-114">managedEBookAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="9829a-114">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="9829a-115">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9829a-115">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="9829a-116">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9829a-116">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="9829a-117">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="9829a-117">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="9829a-118">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9829a-118">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="9829a-119">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9829a-119">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="9829a-120">managedEBookAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="9829a-120">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="9829a-121">なし</span><span class="sxs-lookup"><span data-stu-id="9829a-121">None</span></span>|<span data-ttu-id="9829a-122">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="9829a-122">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="9829a-123">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="9829a-123">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="9829a-124">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="9829a-124">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="9829a-125">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9829a-125">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9829a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9829a-126">Properties</span></span>
|<span data-ttu-id="9829a-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9829a-127">Property</span></span>|<span data-ttu-id="9829a-128">型</span><span class="sxs-lookup"><span data-stu-id="9829a-128">Type</span></span>|<span data-ttu-id="9829a-129">説明</span><span class="sxs-lookup"><span data-stu-id="9829a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9829a-130">id</span><span class="sxs-lookup"><span data-stu-id="9829a-130">id</span></span>|<span data-ttu-id="9829a-131">String</span><span class="sxs-lookup"><span data-stu-id="9829a-131">String</span></span>|<span data-ttu-id="9829a-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9829a-132">Key of the entity.</span></span>|
|<span data-ttu-id="9829a-133">target</span><span class="sxs-lookup"><span data-stu-id="9829a-133">target</span></span>|[<span data-ttu-id="9829a-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9829a-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9829a-135">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="9829a-135">The assignment target for eBook.</span></span>|
|<span data-ttu-id="9829a-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="9829a-136">installIntent</span></span>|[<span data-ttu-id="9829a-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="9829a-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="9829a-138">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="9829a-138">The install intent for eBook.</span></span> <span data-ttu-id="9829a-139">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="9829a-139">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9829a-140">関係</span><span class="sxs-lookup"><span data-stu-id="9829a-140">Relationships</span></span>
<span data-ttu-id="9829a-141">なし</span><span class="sxs-lookup"><span data-stu-id="9829a-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9829a-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9829a-142">JSON Representation</span></span>
<span data-ttu-id="9829a-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9829a-143">Here is a JSON representation of the resource.</span></span>
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




