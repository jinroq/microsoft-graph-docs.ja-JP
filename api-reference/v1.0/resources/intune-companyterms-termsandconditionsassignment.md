---
title: termsAndConditionsAssignment リソース タイプ
description: C) を指定されたグループのポリシーです。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
ms.openlocfilehash: 848998e59f214fc679aba7c27a2a529be05c8adc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022987"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="60eb3-104">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="60eb3-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="60eb3-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60eb3-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60eb3-106">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="60eb3-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="60eb3-107">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="60eb3-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="60eb3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="60eb3-108">Methods</span></span>
|<span data-ttu-id="60eb3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="60eb3-109">Method</span></span>|<span data-ttu-id="60eb3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="60eb3-110">Return Type</span></span>|<span data-ttu-id="60eb3-111">説明</span><span class="sxs-lookup"><span data-stu-id="60eb3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60eb3-112">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="60eb3-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="60eb3-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="60eb3-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="60eb3-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="60eb3-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="60eb3-115">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="60eb3-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="60eb3-117">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="60eb3-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="60eb3-118">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="60eb3-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="60eb3-120">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="60eb3-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="60eb3-121">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="60eb3-122">なし</span><span class="sxs-lookup"><span data-stu-id="60eb3-122">None</span></span>|<span data-ttu-id="60eb3-123">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="60eb3-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="60eb3-124">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="60eb3-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="60eb3-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="60eb3-126">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="60eb3-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60eb3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60eb3-127">Properties</span></span>
|<span data-ttu-id="60eb3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60eb3-128">Property</span></span>|<span data-ttu-id="60eb3-129">型</span><span class="sxs-lookup"><span data-stu-id="60eb3-129">Type</span></span>|<span data-ttu-id="60eb3-130">説明</span><span class="sxs-lookup"><span data-stu-id="60eb3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60eb3-131">id</span><span class="sxs-lookup"><span data-stu-id="60eb3-131">id</span></span>|<span data-ttu-id="60eb3-132">String</span><span class="sxs-lookup"><span data-stu-id="60eb3-132">String</span></span>|<span data-ttu-id="60eb3-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="60eb3-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="60eb3-134">target</span><span class="sxs-lookup"><span data-stu-id="60eb3-134">target</span></span>|[<span data-ttu-id="60eb3-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="60eb3-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="60eb3-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="60eb3-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60eb3-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60eb3-137">Relationships</span></span>
<span data-ttu-id="60eb3-138">なし</span><span class="sxs-lookup"><span data-stu-id="60eb3-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60eb3-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60eb3-139">JSON Representation</span></span>
<span data-ttu-id="60eb3-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="60eb3-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



