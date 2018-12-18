---
title: termsAndConditionsAssignment リソース タイプ
description: C) を指定されたグループのポリシーです。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: tfitzmac
ms.openlocfilehash: a7b0e9deb391b9431be1ed4f282cb6e5a63ced6e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351052"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="9245c-104">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="9245c-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="9245c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9245c-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9245c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9245c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9245c-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9245c-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9245c-108">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="9245c-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="9245c-109">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9245c-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="9245c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="9245c-110">Methods</span></span>
|<span data-ttu-id="9245c-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9245c-111">Method</span></span>|<span data-ttu-id="9245c-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9245c-112">Return Type</span></span>|<span data-ttu-id="9245c-113">説明</span><span class="sxs-lookup"><span data-stu-id="9245c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9245c-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="9245c-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="9245c-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9245c-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="9245c-116">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9245c-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="9245c-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="9245c-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="9245c-119">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9245c-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="9245c-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="9245c-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="9245c-122">新しい [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9245c-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="9245c-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="9245c-124">なし</span><span class="sxs-lookup"><span data-stu-id="9245c-124">None</span></span>|<span data-ttu-id="9245c-125">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="9245c-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="9245c-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="9245c-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="9245c-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="9245c-128">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9245c-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9245c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9245c-129">Properties</span></span>
|<span data-ttu-id="9245c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9245c-130">Property</span></span>|<span data-ttu-id="9245c-131">種類</span><span class="sxs-lookup"><span data-stu-id="9245c-131">Type</span></span>|<span data-ttu-id="9245c-132">説明</span><span class="sxs-lookup"><span data-stu-id="9245c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9245c-133">ID</span><span class="sxs-lookup"><span data-stu-id="9245c-133">id</span></span>|<span data-ttu-id="9245c-134">String</span><span class="sxs-lookup"><span data-stu-id="9245c-134">String</span></span>|<span data-ttu-id="9245c-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="9245c-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9245c-136">target</span><span class="sxs-lookup"><span data-stu-id="9245c-136">target</span></span>|[<span data-ttu-id="9245c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9245c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9245c-138">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="9245c-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9245c-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9245c-139">Relationships</span></span>
<span data-ttu-id="9245c-140">なし</span><span class="sxs-lookup"><span data-stu-id="9245c-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9245c-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9245c-141">JSON Representation</span></span>
<span data-ttu-id="9245c-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9245c-142">Here is a JSON representation of the resource.</span></span>
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





