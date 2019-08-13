---
title: termsAndConditionsGroupAssignment リソースの種類
description: TermsAndConditionsGroupAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 121ac9d46450e88d826aa59ffde0216a7aac5231
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335009"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="efd26-104">termsAndConditionsGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="efd26-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="efd26-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efd26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efd26-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efd26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd26-107">TermsAndConditionsGroupAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="efd26-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="efd26-108">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="efd26-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="efd26-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="efd26-109">Methods</span></span>
|<span data-ttu-id="efd26-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="efd26-110">Method</span></span>|<span data-ttu-id="efd26-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="efd26-111">Return Type</span></span>|<span data-ttu-id="efd26-112">説明</span><span class="sxs-lookup"><span data-stu-id="efd26-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="efd26-113">リスト termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="efd26-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="efd26-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="efd26-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="efd26-115">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="efd26-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="efd26-116">TermsAndConditionsGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="efd26-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="efd26-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efd26-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="efd26-118">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="efd26-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="efd26-119">TermsAndConditionsGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="efd26-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="efd26-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efd26-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="efd26-121">新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="efd26-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="efd26-122">TermsAndConditionsGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="efd26-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="efd26-123">None</span><span class="sxs-lookup"><span data-stu-id="efd26-123">None</span></span>|<span data-ttu-id="efd26-124">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="efd26-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="efd26-125">TermsAndConditionsGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="efd26-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="efd26-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="efd26-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="efd26-127">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="efd26-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="efd26-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efd26-128">Properties</span></span>
|<span data-ttu-id="efd26-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efd26-129">Property</span></span>|<span data-ttu-id="efd26-130">型</span><span class="sxs-lookup"><span data-stu-id="efd26-130">Type</span></span>|<span data-ttu-id="efd26-131">説明</span><span class="sxs-lookup"><span data-stu-id="efd26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd26-132">id</span><span class="sxs-lookup"><span data-stu-id="efd26-132">id</span></span>|<span data-ttu-id="efd26-133">String</span><span class="sxs-lookup"><span data-stu-id="efd26-133">String</span></span>|<span data-ttu-id="efd26-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="efd26-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="efd26-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="efd26-135">targetGroupId</span></span>|<span data-ttu-id="efd26-136">String</span><span class="sxs-lookup"><span data-stu-id="efd26-136">String</span></span>|<span data-ttu-id="efd26-137">T&C ポリシーが割り当てられているグループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="efd26-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efd26-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="efd26-138">Relationships</span></span>
|<span data-ttu-id="efd26-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="efd26-139">Relationship</span></span>|<span data-ttu-id="efd26-140">型</span><span class="sxs-lookup"><span data-stu-id="efd26-140">Type</span></span>|<span data-ttu-id="efd26-141">説明</span><span class="sxs-lookup"><span data-stu-id="efd26-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd26-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="efd26-142">termsAndConditions</span></span>|[<span data-ttu-id="efd26-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="efd26-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="efd26-144">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="efd26-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efd26-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="efd26-145">JSON Representation</span></span>
<span data-ttu-id="efd26-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="efd26-146">Here is a JSON representation of the resource.</span></span>
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



