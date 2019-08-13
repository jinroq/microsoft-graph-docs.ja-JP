---
title: managedEBookAssignment リソースの種類
description: グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4eaecbfcc9162ab549d8da17460bdced873d0dd9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335116"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="abba3-103">managedEBookAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abba3-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="abba3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abba3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abba3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="abba3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abba3-106">グループへの電子ブックの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="abba3-106">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="abba3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="abba3-107">Methods</span></span>
|<span data-ttu-id="abba3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="abba3-108">Method</span></span>|<span data-ttu-id="abba3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="abba3-109">Return Type</span></span>|<span data-ttu-id="abba3-110">説明</span><span class="sxs-lookup"><span data-stu-id="abba3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="abba3-111">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="abba3-111">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="abba3-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="abba3-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="abba3-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="abba3-113">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="abba3-114">managedEBookAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="abba3-114">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="abba3-115">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="abba3-115">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="abba3-116">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="abba3-116">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="abba3-117">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="abba3-117">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="abba3-118">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="abba3-118">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="abba3-119">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="abba3-119">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="abba3-120">managedEBookAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="abba3-120">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="abba3-121">なし</span><span class="sxs-lookup"><span data-stu-id="abba3-121">None</span></span>|<span data-ttu-id="abba3-122">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="abba3-122">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="abba3-123">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="abba3-123">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="abba3-124">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="abba3-124">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="abba3-125">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="abba3-125">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="abba3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abba3-126">Properties</span></span>
|<span data-ttu-id="abba3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abba3-127">Property</span></span>|<span data-ttu-id="abba3-128">型</span><span class="sxs-lookup"><span data-stu-id="abba3-128">Type</span></span>|<span data-ttu-id="abba3-129">説明</span><span class="sxs-lookup"><span data-stu-id="abba3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abba3-130">id</span><span class="sxs-lookup"><span data-stu-id="abba3-130">id</span></span>|<span data-ttu-id="abba3-131">String</span><span class="sxs-lookup"><span data-stu-id="abba3-131">String</span></span>|<span data-ttu-id="abba3-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="abba3-132">Key of the entity.</span></span>|
|<span data-ttu-id="abba3-133">target</span><span class="sxs-lookup"><span data-stu-id="abba3-133">target</span></span>|[<span data-ttu-id="abba3-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="abba3-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="abba3-135">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="abba3-135">The assignment target for eBook.</span></span>|
|<span data-ttu-id="abba3-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="abba3-136">installIntent</span></span>|[<span data-ttu-id="abba3-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="abba3-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="abba3-138">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="abba3-138">The install intent for eBook.</span></span> <span data-ttu-id="abba3-139">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="abba3-139">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="abba3-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="abba3-140">Relationships</span></span>
<span data-ttu-id="abba3-141">なし</span><span class="sxs-lookup"><span data-stu-id="abba3-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="abba3-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abba3-142">JSON Representation</span></span>
<span data-ttu-id="abba3-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="abba3-143">Here is a JSON representation of the resource.</span></span>
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



