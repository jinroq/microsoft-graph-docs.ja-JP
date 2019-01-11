---
title: termsAndConditionsGroupAssignment リソースの種類
description: C) を指定されたグループのポリシーです。 グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9ae49e1223c4b74fb8da8da7f5b42533fd33c8c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874222"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="35678-104">termsAndConditionsGroupAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35678-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="35678-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35678-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35678-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35678-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35678-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35678-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35678-108">TermsAndConditionsGroupAssignment エンティティは、指定された条項および条件 (T & C) ポリシーを指定したグループの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="35678-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="35678-109">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="35678-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="35678-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="35678-110">Methods</span></span>
|<span data-ttu-id="35678-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="35678-111">Method</span></span>|<span data-ttu-id="35678-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35678-112">Return Type</span></span>|<span data-ttu-id="35678-113">説明</span><span class="sxs-lookup"><span data-stu-id="35678-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35678-114">リスト termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="35678-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="35678-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="35678-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="35678-116">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="35678-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="35678-117">TermsAndConditionsGroupAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="35678-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="35678-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="35678-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="35678-119">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35678-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="35678-120">TermsAndConditionsGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="35678-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="35678-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="35678-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="35678-122">新しい[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="35678-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="35678-123">TermsAndConditionsGroupAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="35678-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="35678-124">なし</span><span class="sxs-lookup"><span data-stu-id="35678-124">None</span></span>|<span data-ttu-id="35678-125">の[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="35678-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="35678-126">TermsAndConditionsGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="35678-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="35678-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="35678-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="35678-128">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="35678-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35678-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35678-129">Properties</span></span>
|<span data-ttu-id="35678-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35678-130">Property</span></span>|<span data-ttu-id="35678-131">種類</span><span class="sxs-lookup"><span data-stu-id="35678-131">Type</span></span>|<span data-ttu-id="35678-132">説明</span><span class="sxs-lookup"><span data-stu-id="35678-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35678-133">ID</span><span class="sxs-lookup"><span data-stu-id="35678-133">id</span></span>|<span data-ttu-id="35678-134">String</span><span class="sxs-lookup"><span data-stu-id="35678-134">String</span></span>|<span data-ttu-id="35678-135">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="35678-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="35678-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="35678-136">targetGroupId</span></span>|<span data-ttu-id="35678-137">String</span><span class="sxs-lookup"><span data-stu-id="35678-137">String</span></span>|<span data-ttu-id="35678-138">T & C のポリシーが割り当てられているグループの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="35678-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35678-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35678-139">Relationships</span></span>
|<span data-ttu-id="35678-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35678-140">Relationship</span></span>|<span data-ttu-id="35678-141">型</span><span class="sxs-lookup"><span data-stu-id="35678-141">Type</span></span>|<span data-ttu-id="35678-142">説明</span><span class="sxs-lookup"><span data-stu-id="35678-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35678-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="35678-143">termsAndConditions</span></span>|[<span data-ttu-id="35678-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="35678-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="35678-145">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="35678-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35678-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35678-146">JSON Representation</span></span>
<span data-ttu-id="35678-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35678-147">Here is a JSON representation of the resource.</span></span>
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





