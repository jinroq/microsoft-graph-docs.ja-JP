---
title: managedEBookAssignment リソースの種類
description: グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 325e094698bb2ccbfaf4c41dd46f71c461c8681f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541382"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="f4536-103">managedEBookAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4536-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="f4536-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4536-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4536-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4536-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4536-106">グループへの電子ブックの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4536-106">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="f4536-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4536-107">Methods</span></span>
|<span data-ttu-id="f4536-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4536-108">Method</span></span>|<span data-ttu-id="f4536-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f4536-109">Return Type</span></span>|<span data-ttu-id="f4536-110">説明</span><span class="sxs-lookup"><span data-stu-id="f4536-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4536-111">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="f4536-111">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="f4536-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f4536-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="f4536-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f4536-113">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="f4536-114">managedEBookAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="f4536-114">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="f4536-115">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="f4536-115">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="f4536-116">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4536-116">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="f4536-117">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="f4536-117">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="f4536-118">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="f4536-118">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="f4536-119">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f4536-119">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="f4536-120">managedEBookAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="f4536-120">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="f4536-121">なし</span><span class="sxs-lookup"><span data-stu-id="f4536-121">None</span></span>|<span data-ttu-id="f4536-122">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f4536-122">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="f4536-123">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="f4536-123">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="f4536-124">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="f4536-124">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="f4536-125">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4536-125">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4536-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4536-126">Properties</span></span>
|<span data-ttu-id="f4536-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4536-127">Property</span></span>|<span data-ttu-id="f4536-128">型</span><span class="sxs-lookup"><span data-stu-id="f4536-128">Type</span></span>|<span data-ttu-id="f4536-129">説明</span><span class="sxs-lookup"><span data-stu-id="f4536-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4536-130">id</span><span class="sxs-lookup"><span data-stu-id="f4536-130">id</span></span>|<span data-ttu-id="f4536-131">String</span><span class="sxs-lookup"><span data-stu-id="f4536-131">String</span></span>|<span data-ttu-id="f4536-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f4536-132">Key of the entity.</span></span>|
|<span data-ttu-id="f4536-133">target</span><span class="sxs-lookup"><span data-stu-id="f4536-133">target</span></span>|[<span data-ttu-id="f4536-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f4536-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f4536-135">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="f4536-135">The assignment target for eBook.</span></span>|
|<span data-ttu-id="f4536-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="f4536-136">installIntent</span></span>|[<span data-ttu-id="f4536-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="f4536-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f4536-138">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="f4536-138">The install intent for eBook.</span></span> <span data-ttu-id="f4536-139">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="f4536-139">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4536-140">関係</span><span class="sxs-lookup"><span data-stu-id="f4536-140">Relationships</span></span>
<span data-ttu-id="f4536-141">なし</span><span class="sxs-lookup"><span data-stu-id="f4536-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4536-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4536-142">JSON Representation</span></span>
<span data-ttu-id="f4536-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4536-143">Here is a JSON representation of the resource.</span></span>
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





