---
title: termsAndConditionsGroupAssignment リソースの種類
description: termsAndConditionsGroupAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f3518dcc31bf703d3fe42e6bab15d5731d5beb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463526"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="034c1-104">termsAndConditionsGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="034c1-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="034c1-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="034c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="034c1-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="034c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="034c1-107">termsAndConditionsGroupAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="034c1-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="034c1-108">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="034c1-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="034c1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="034c1-109">Methods</span></span>
|<span data-ttu-id="034c1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="034c1-110">Method</span></span>|<span data-ttu-id="034c1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="034c1-111">Return Type</span></span>|<span data-ttu-id="034c1-112">説明</span><span class="sxs-lookup"><span data-stu-id="034c1-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="034c1-113">リスト termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="034c1-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="034c1-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="034c1-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="034c1-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="034c1-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="034c1-116">termsAndConditionsGroupAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="034c1-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="034c1-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="034c1-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="034c1-118">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="034c1-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="034c1-119">termsAndConditionsGroupAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="034c1-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="034c1-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="034c1-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="034c1-121">新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="034c1-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="034c1-122">termsAndConditionsGroupAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="034c1-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="034c1-123">なし</span><span class="sxs-lookup"><span data-stu-id="034c1-123">None</span></span>|<span data-ttu-id="034c1-124">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="034c1-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="034c1-125">termsAndConditionsGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="034c1-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="034c1-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="034c1-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="034c1-127">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="034c1-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="034c1-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="034c1-128">Properties</span></span>
|<span data-ttu-id="034c1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="034c1-129">Property</span></span>|<span data-ttu-id="034c1-130">型</span><span class="sxs-lookup"><span data-stu-id="034c1-130">Type</span></span>|<span data-ttu-id="034c1-131">説明</span><span class="sxs-lookup"><span data-stu-id="034c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="034c1-132">id</span><span class="sxs-lookup"><span data-stu-id="034c1-132">id</span></span>|<span data-ttu-id="034c1-133">String</span><span class="sxs-lookup"><span data-stu-id="034c1-133">String</span></span>|<span data-ttu-id="034c1-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="034c1-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="034c1-135">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="034c1-135">targetGroupId</span></span>|<span data-ttu-id="034c1-136">String</span><span class="sxs-lookup"><span data-stu-id="034c1-136">String</span></span>|<span data-ttu-id="034c1-137">T&C ポリシーが割り当てられているグループの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="034c1-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="034c1-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="034c1-138">Relationships</span></span>
|<span data-ttu-id="034c1-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="034c1-139">Relationship</span></span>|<span data-ttu-id="034c1-140">型</span><span class="sxs-lookup"><span data-stu-id="034c1-140">Type</span></span>|<span data-ttu-id="034c1-141">説明</span><span class="sxs-lookup"><span data-stu-id="034c1-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="034c1-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="034c1-142">termsAndConditions</span></span>|[<span data-ttu-id="034c1-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="034c1-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="034c1-144">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="034c1-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="034c1-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="034c1-145">JSON Representation</span></span>
<span data-ttu-id="034c1-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="034c1-146">Here is a JSON representation of the resource.</span></span>
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





