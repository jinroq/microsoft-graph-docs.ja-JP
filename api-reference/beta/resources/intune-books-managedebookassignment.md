---
title: managedEBookAssignment リソースの種類
description: グループへの電子ブックの割り当てに使用されるプロパティが含まれています。
ms.openlocfilehash: 7c4ddba8f4a0c115be18f760d6874a6f54d429e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069910"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="7481e-103">managedEBookAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7481e-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="7481e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7481e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7481e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7481e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7481e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7481e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7481e-107">グループへの電子ブックの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7481e-107">Contains properties used to assign a eBook to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="7481e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7481e-108">Methods</span></span>
|<span data-ttu-id="7481e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7481e-109">Method</span></span>|<span data-ttu-id="7481e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7481e-110">Return Type</span></span>|<span data-ttu-id="7481e-111">説明</span><span class="sxs-lookup"><span data-stu-id="7481e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7481e-112">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="7481e-112">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="7481e-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7481e-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="7481e-114">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7481e-114">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="7481e-115">managedEBookAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="7481e-115">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="7481e-116">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7481e-116">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="7481e-117">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7481e-117">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="7481e-118">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="7481e-118">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="7481e-119">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7481e-119">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="7481e-120">新しい [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7481e-120">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="7481e-121">managedEBookAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="7481e-121">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="7481e-122">なし</span><span class="sxs-lookup"><span data-stu-id="7481e-122">None</span></span>|<span data-ttu-id="7481e-123">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7481e-123">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="7481e-124">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7481e-124">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="7481e-125">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7481e-125">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="7481e-126">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7481e-126">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7481e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7481e-127">Properties</span></span>
|<span data-ttu-id="7481e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7481e-128">Property</span></span>|<span data-ttu-id="7481e-129">型</span><span class="sxs-lookup"><span data-stu-id="7481e-129">Type</span></span>|<span data-ttu-id="7481e-130">説明</span><span class="sxs-lookup"><span data-stu-id="7481e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7481e-131">id</span><span class="sxs-lookup"><span data-stu-id="7481e-131">id</span></span>|<span data-ttu-id="7481e-132">String</span><span class="sxs-lookup"><span data-stu-id="7481e-132">String</span></span>|<span data-ttu-id="7481e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7481e-133">Key of the entity.</span></span>|
|<span data-ttu-id="7481e-134">target</span><span class="sxs-lookup"><span data-stu-id="7481e-134">target</span></span>|[<span data-ttu-id="7481e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7481e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7481e-136">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="7481e-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="7481e-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="7481e-137">installIntent</span></span>|[<span data-ttu-id="7481e-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="7481e-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7481e-139">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="7481e-139">The install intent for eBook.</span></span> <span data-ttu-id="7481e-140">可能な値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="7481e-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7481e-141">関係</span><span class="sxs-lookup"><span data-stu-id="7481e-141">Relationships</span></span>
<span data-ttu-id="7481e-142">なし</span><span class="sxs-lookup"><span data-stu-id="7481e-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7481e-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7481e-143">JSON Representation</span></span>
<span data-ttu-id="7481e-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7481e-144">Here is a JSON representation of the resource.</span></span>
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





