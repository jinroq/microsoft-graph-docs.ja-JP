---
title: termsAndConditionsGroupAssignment リソースの種類
description: C) を指定されたグループのポリシーです。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
ms.openlocfilehash: 071cd73ba36aaab74c7f5c36522c03014711286e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072083"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="0a5ad-104">termsAndConditionsGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a5ad-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="0a5ad-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a5ad-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a5ad-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a5ad-108">TermsAndConditionsGroupAssignment エンティティは、指定された条項および条件 (T & C) ポリシーを指定したグループの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="0a5ad-109">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="0a5ad-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a5ad-110">Methods</span></span>
|<span data-ttu-id="0a5ad-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a5ad-111">Method</span></span>|<span data-ttu-id="0a5ad-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a5ad-112">Return Type</span></span>|<span data-ttu-id="0a5ad-113">説明</span><span class="sxs-lookup"><span data-stu-id="0a5ad-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a5ad-114">リスト termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="0a5ad-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="0a5ad-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a5ad-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="0a5ad-116">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="0a5ad-117">TermsAndConditionsGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="0a5ad-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0a5ad-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="0a5ad-119">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="0a5ad-120">TermsAndConditionsGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="0a5ad-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0a5ad-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="0a5ad-122">新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="0a5ad-123">TermsAndConditionsGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="0a5ad-124">なし</span><span class="sxs-lookup"><span data-stu-id="0a5ad-124">None</span></span>|<span data-ttu-id="0a5ad-125">の[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="0a5ad-126">TermsAndConditionsGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="0a5ad-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0a5ad-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="0a5ad-128">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a5ad-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a5ad-129">Properties</span></span>
|<span data-ttu-id="0a5ad-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a5ad-130">Property</span></span>|<span data-ttu-id="0a5ad-131">型</span><span class="sxs-lookup"><span data-stu-id="0a5ad-131">Type</span></span>|<span data-ttu-id="0a5ad-132">説明</span><span class="sxs-lookup"><span data-stu-id="0a5ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a5ad-133">id</span><span class="sxs-lookup"><span data-stu-id="0a5ad-133">id</span></span>|<span data-ttu-id="0a5ad-134">String</span><span class="sxs-lookup"><span data-stu-id="0a5ad-134">String</span></span>|<span data-ttu-id="0a5ad-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0a5ad-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="0a5ad-136">targetGroupId</span></span>|<span data-ttu-id="0a5ad-137">String</span><span class="sxs-lookup"><span data-stu-id="0a5ad-137">String</span></span>|<span data-ttu-id="0a5ad-138">T & C のポリシーが割り当てられているグループの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a5ad-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a5ad-139">Relationships</span></span>
|<span data-ttu-id="0a5ad-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a5ad-140">Relationship</span></span>|<span data-ttu-id="0a5ad-141">型</span><span class="sxs-lookup"><span data-stu-id="0a5ad-141">Type</span></span>|<span data-ttu-id="0a5ad-142">説明</span><span class="sxs-lookup"><span data-stu-id="0a5ad-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a5ad-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="0a5ad-143">termsAndConditions</span></span>|[<span data-ttu-id="0a5ad-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="0a5ad-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="0a5ad-145">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a5ad-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a5ad-146">JSON Representation</span></span>
<span data-ttu-id="0a5ad-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a5ad-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





