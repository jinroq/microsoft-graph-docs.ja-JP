---
title: termsAndConditionsAssignment リソース タイプ
description: C) を指定されたグループのポリシーです。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba87e7b5f3b39f20befb1536f3a87583437eeee3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889370"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="fd028-104">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="fd028-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="fd028-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd028-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd028-106">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="fd028-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="fd028-107">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd028-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="fd028-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd028-108">Methods</span></span>
|<span data-ttu-id="fd028-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fd028-109">Method</span></span>|<span data-ttu-id="fd028-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fd028-110">Return Type</span></span>|<span data-ttu-id="fd028-111">説明</span><span class="sxs-lookup"><span data-stu-id="fd028-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd028-112">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="fd028-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="fd028-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fd028-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="fd028-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fd028-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="fd028-115">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="fd028-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="fd028-117">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fd028-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="fd028-118">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="fd028-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="fd028-120">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fd028-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="fd028-121">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="fd028-122">なし</span><span class="sxs-lookup"><span data-stu-id="fd028-122">None</span></span>|<span data-ttu-id="fd028-123">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fd028-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="fd028-124">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="fd028-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="fd028-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="fd028-126">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd028-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd028-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd028-127">Properties</span></span>
|<span data-ttu-id="fd028-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd028-128">Property</span></span>|<span data-ttu-id="fd028-129">種類</span><span class="sxs-lookup"><span data-stu-id="fd028-129">Type</span></span>|<span data-ttu-id="fd028-130">説明</span><span class="sxs-lookup"><span data-stu-id="fd028-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd028-131">ID</span><span class="sxs-lookup"><span data-stu-id="fd028-131">id</span></span>|<span data-ttu-id="fd028-132">String</span><span class="sxs-lookup"><span data-stu-id="fd028-132">String</span></span>|<span data-ttu-id="fd028-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="fd028-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fd028-134">target</span><span class="sxs-lookup"><span data-stu-id="fd028-134">target</span></span>|[<span data-ttu-id="fd028-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fd028-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fd028-136">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="fd028-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd028-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd028-137">Relationships</span></span>
<span data-ttu-id="fd028-138">なし</span><span class="sxs-lookup"><span data-stu-id="fd028-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd028-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd028-139">JSON Representation</span></span>
<span data-ttu-id="fd028-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd028-140">Here is a JSON representation of the resource.</span></span>
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



