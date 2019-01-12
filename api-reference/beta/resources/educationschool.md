---
title: educationSchool リソースの種類
description: '学校。 現時点で、**educationSchool** リソースは administrativeUnit リソースと一致していて、同じ ID を共有しています。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 17a5c3ad2f28e802bb6cad3a97d1cb723b3407d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918246"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="e747d-104">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e747d-104">educationSchool resource type</span></span>

> <span data-ttu-id="e747d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e747d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e747d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e747d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e747d-107">学校。</span><span class="sxs-lookup"><span data-stu-id="e747d-107">A school.</span></span> <span data-ttu-id="e747d-108">現時点で、**educationSchool** リソースは [administrativeUnit](administrativeunit.md) リソースと一致していて、同じ ID を共有しています。</span><span class="sxs-lookup"><span data-stu-id="e747d-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="e747d-109">このリソースは、[educationOrganization](educationorganization.md) のサブタイプです。</span><span class="sxs-lookup"><span data-stu-id="e747d-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="e747d-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e747d-110">Methods</span></span>

| <span data-ttu-id="e747d-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="e747d-111">Method</span></span>           | <span data-ttu-id="e747d-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e747d-112">Return Type</span></span>    |<span data-ttu-id="e747d-113">説明</span><span class="sxs-lookup"><span data-stu-id="e747d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e747d-114">Get</span><span class="sxs-lookup"><span data-stu-id="e747d-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="e747d-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e747d-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="e747d-116">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e747d-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="e747d-117">Add class</span><span class="sxs-lookup"><span data-stu-id="e747d-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="e747d-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="e747d-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="e747d-119">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="e747d-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="e747d-120">List classes</span><span class="sxs-lookup"><span data-stu-id="e747d-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="e747d-121">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e747d-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e747d-122">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e747d-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="e747d-123">Remove class</span><span class="sxs-lookup"><span data-stu-id="e747d-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="e747d-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="e747d-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="e747d-125">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="e747d-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="e747d-126">Add user</span><span class="sxs-lookup"><span data-stu-id="e747d-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="e747d-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="e747d-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e747d-128">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="e747d-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="e747d-129">List users</span><span class="sxs-lookup"><span data-stu-id="e747d-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="e747d-130">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e747d-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e747d-131">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e747d-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="e747d-132">Remove user</span><span class="sxs-lookup"><span data-stu-id="e747d-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="e747d-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="e747d-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e747d-134">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="e747d-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="e747d-135">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="e747d-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="e747d-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="e747d-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="e747d-137">この **educationSchool** に対応する **administrativeUnit** を取得します。</span><span class="sxs-lookup"><span data-stu-id="e747d-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="e747d-138">Update</span><span class="sxs-lookup"><span data-stu-id="e747d-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="e747d-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e747d-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="e747d-140">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e747d-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="e747d-141">Delete</span><span class="sxs-lookup"><span data-stu-id="e747d-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="e747d-142">なし</span><span class="sxs-lookup"><span data-stu-id="e747d-142">None</span></span> |<span data-ttu-id="e747d-143">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e747d-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e747d-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e747d-144">Properties</span></span>
| <span data-ttu-id="e747d-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e747d-145">Property</span></span>     | <span data-ttu-id="e747d-146">種類</span><span class="sxs-lookup"><span data-stu-id="e747d-146">Type</span></span>   |<span data-ttu-id="e747d-147">説明</span><span class="sxs-lookup"><span data-stu-id="e747d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e747d-148">ID</span><span class="sxs-lookup"><span data-stu-id="e747d-148">id</span></span>|<span data-ttu-id="e747d-149">String</span><span class="sxs-lookup"><span data-stu-id="e747d-149">String</span></span>|<span data-ttu-id="e747d-150">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="e747d-150">GUID of this school.</span></span>|
|<span data-ttu-id="e747d-151">displayName</span><span class="sxs-lookup"><span data-stu-id="e747d-151">displayName</span></span>| <span data-ttu-id="e747d-152">String</span><span class="sxs-lookup"><span data-stu-id="e747d-152">String</span></span>| <span data-ttu-id="e747d-153">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="e747d-153">Display name of the school.</span></span>| 
|<span data-ttu-id="e747d-154">説明</span><span class="sxs-lookup"><span data-stu-id="e747d-154">description</span></span>| <span data-ttu-id="e747d-155">String</span><span class="sxs-lookup"><span data-stu-id="e747d-155">String</span></span> | <span data-ttu-id="e747d-156">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="e747d-156">Description of the school.</span></span>| 
|<span data-ttu-id="e747d-157">status</span><span class="sxs-lookup"><span data-stu-id="e747d-157">status</span></span>| <span data-ttu-id="e747d-158">文字列</span><span class="sxs-lookup"><span data-stu-id="e747d-158">string</span></span>| <span data-ttu-id="e747d-159">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e747d-159">Read-Only.</span></span> <span data-ttu-id="e747d-160">使用可能な値: `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="e747d-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="e747d-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="e747d-161">externalSource</span></span>| <span data-ttu-id="e747d-162">文字列</span><span class="sxs-lookup"><span data-stu-id="e747d-162">string</span></span>| <span data-ttu-id="e747d-163">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e747d-163">Read-Only.</span></span>  <span data-ttu-id="e747d-164">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e747d-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e747d-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="e747d-165">principalEmail</span></span>| <span data-ttu-id="e747d-166">String</span><span class="sxs-lookup"><span data-stu-id="e747d-166">String</span></span>| <span data-ttu-id="e747d-167">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="e747d-167">Email address of the principal.</span></span>|
|<span data-ttu-id="e747d-168">principalName</span><span class="sxs-lookup"><span data-stu-id="e747d-168">principalName</span></span>| <span data-ttu-id="e747d-169">String</span><span class="sxs-lookup"><span data-stu-id="e747d-169">String</span></span> | <span data-ttu-id="e747d-170">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="e747d-170">Name of the principal.</span></span>|
|<span data-ttu-id="e747d-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="e747d-171">externalPrincipalId</span></span>| <span data-ttu-id="e747d-172">String</span><span class="sxs-lookup"><span data-stu-id="e747d-172">String</span></span> | <span data-ttu-id="e747d-173">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="e747d-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="e747d-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="e747d-174">highestGrade</span></span>|<span data-ttu-id="e747d-175">String</span><span class="sxs-lookup"><span data-stu-id="e747d-175">String</span></span>| <span data-ttu-id="e747d-176">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="e747d-176">Highest grade taught.</span></span> |
|<span data-ttu-id="e747d-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="e747d-177">lowestGrade</span></span>|<span data-ttu-id="e747d-178">String</span><span class="sxs-lookup"><span data-stu-id="e747d-178">String</span></span>| <span data-ttu-id="e747d-179">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="e747d-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="e747d-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="e747d-180">schoolNumber</span></span>|<span data-ttu-id="e747d-181">String</span><span class="sxs-lookup"><span data-stu-id="e747d-181">String</span></span>| <span data-ttu-id="e747d-182">学校番号。</span><span class="sxs-lookup"><span data-stu-id="e747d-182">School Number.</span></span>|
|<span data-ttu-id="e747d-183">externalId</span><span class="sxs-lookup"><span data-stu-id="e747d-183">externalId</span></span>|<span data-ttu-id="e747d-184">String</span><span class="sxs-lookup"><span data-stu-id="e747d-184">String</span></span>| <span data-ttu-id="e747d-185">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="e747d-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="e747d-186">phone</span><span class="sxs-lookup"><span data-stu-id="e747d-186">phone</span></span>|<span data-ttu-id="e747d-187">String</span><span class="sxs-lookup"><span data-stu-id="e747d-187">String</span></span>| <span data-ttu-id="e747d-188">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="e747d-188">Phone number of school.</span></span> |
|<span data-ttu-id="e747d-189">fax</span><span class="sxs-lookup"><span data-stu-id="e747d-189">fax</span></span>|<span data-ttu-id="e747d-190">String</span><span class="sxs-lookup"><span data-stu-id="e747d-190">String</span></span>| <span data-ttu-id="e747d-191">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="e747d-191">Fax number of school.</span></span> |
|<span data-ttu-id="e747d-192">address</span><span class="sxs-lookup"><span data-stu-id="e747d-192">address</span></span>|[<span data-ttu-id="e747d-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e747d-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="e747d-194">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="e747d-194">Address of the school.</span></span>|
|<span data-ttu-id="e747d-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="e747d-195">createdBy</span></span>|[<span data-ttu-id="e747d-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="e747d-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="e747d-197">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="e747d-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="e747d-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e747d-198">Relationships</span></span>
| <span data-ttu-id="e747d-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e747d-199">Relationship</span></span> | <span data-ttu-id="e747d-200">型</span><span class="sxs-lookup"><span data-stu-id="e747d-200">Type</span></span>   |<span data-ttu-id="e747d-201">説明</span><span class="sxs-lookup"><span data-stu-id="e747d-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e747d-202">classes</span><span class="sxs-lookup"><span data-stu-id="e747d-202">classes</span></span>|<span data-ttu-id="e747d-203">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e747d-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e747d-204">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="e747d-204">Classes taught at the school.</span></span> <span data-ttu-id="e747d-205">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e747d-205">Nullable.</span></span>|
|<span data-ttu-id="e747d-206">users</span><span class="sxs-lookup"><span data-stu-id="e747d-206">users</span></span>|<span data-ttu-id="e747d-207">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e747d-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e747d-208">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="e747d-208">Users in the school.</span></span> <span data-ttu-id="e747d-209">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e747d-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e747d-210">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e747d-210">JSON representation</span></span>

<span data-ttu-id="e747d-211">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e747d-211">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
