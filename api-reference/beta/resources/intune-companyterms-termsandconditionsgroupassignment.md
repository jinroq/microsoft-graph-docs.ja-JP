---
title: termsAndConditionsGroupAssignment リソースの種類
description: TermsAndConditionsGroupAssignment エンティティの割り当てを表す、条項および条件 (T&C) を指定する特定のグループ ポリシー。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cdb629c380898af078bf0b5eaeb3c39344a5657
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418576"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="5b14c-104">termsAndConditionsGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b14c-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="5b14c-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b14c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b14c-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b14c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b14c-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b14c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b14c-108">TermsAndConditionsGroupAssignment エンティティの割り当てを表す、条項および条件 (T&C) を指定する特定のグループ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="5b14c-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="5b14c-109">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b14c-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="5b14c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b14c-110">Methods</span></span>
|<span data-ttu-id="5b14c-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b14c-111">Method</span></span>|<span data-ttu-id="5b14c-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5b14c-112">Return Type</span></span>|<span data-ttu-id="5b14c-113">説明</span><span class="sxs-lookup"><span data-stu-id="5b14c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5b14c-114">リスト termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="5b14c-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="5b14c-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5b14c-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="5b14c-116">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="5b14c-117">TermsAndConditionsGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="5b14c-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="5b14c-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="5b14c-119">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b14c-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="5b14c-120">TermsAndConditionsGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="5b14c-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="5b14c-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="5b14c-122">新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="5b14c-123">TermsAndConditionsGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="5b14c-124">なし</span><span class="sxs-lookup"><span data-stu-id="5b14c-124">None</span></span>|<span data-ttu-id="5b14c-125">の[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="5b14c-126">TermsAndConditionsGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="5b14c-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="5b14c-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="5b14c-128">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b14c-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b14c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b14c-129">Properties</span></span>
|<span data-ttu-id="5b14c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b14c-130">Property</span></span>|<span data-ttu-id="5b14c-131">型</span><span class="sxs-lookup"><span data-stu-id="5b14c-131">Type</span></span>|<span data-ttu-id="5b14c-132">説明</span><span class="sxs-lookup"><span data-stu-id="5b14c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b14c-133">id</span><span class="sxs-lookup"><span data-stu-id="5b14c-133">id</span></span>|<span data-ttu-id="5b14c-134">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-134">String</span></span>|<span data-ttu-id="5b14c-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5b14c-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5b14c-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="5b14c-136">targetGroupId</span></span>|<span data-ttu-id="5b14c-137">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-137">String</span></span>|<span data-ttu-id="5b14c-138">T&C ポリシーが割り当てられているグループの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5b14c-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b14c-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b14c-139">Relationships</span></span>
|<span data-ttu-id="5b14c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b14c-140">Relationship</span></span>|<span data-ttu-id="5b14c-141">型</span><span class="sxs-lookup"><span data-stu-id="5b14c-141">Type</span></span>|<span data-ttu-id="5b14c-142">説明</span><span class="sxs-lookup"><span data-stu-id="5b14c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b14c-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="5b14c-143">termsAndConditions</span></span>|[<span data-ttu-id="5b14c-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="5b14c-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="5b14c-145">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="5b14c-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b14c-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b14c-146">JSON Representation</span></span>
<span data-ttu-id="5b14c-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b14c-147">Here is a JSON representation of the resource.</span></span>
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




