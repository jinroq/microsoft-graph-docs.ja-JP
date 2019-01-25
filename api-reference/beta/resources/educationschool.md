---
title: educationSchool リソースの種類
description: '学校。 現時点で、**educationSchool** リソースは administrativeUnit リソースと一致していて、同じ ID を共有しています。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512543"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="c6818-104">educationSchool リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c6818-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6818-105">学校。</span><span class="sxs-lookup"><span data-stu-id="c6818-105">A school.</span></span> <span data-ttu-id="c6818-106">現時点で、**educationSchool** リソースは [administrativeUnit](administrativeunit.md) リソースと一致していて、同じ ID を共有しています。</span><span class="sxs-lookup"><span data-stu-id="c6818-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="c6818-107">このリソースは、[educationOrganization](educationorganization.md) のサブタイプです。</span><span class="sxs-lookup"><span data-stu-id="c6818-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="c6818-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6818-108">Methods</span></span>

| <span data-ttu-id="c6818-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6818-109">Method</span></span>           | <span data-ttu-id="c6818-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c6818-110">Return Type</span></span>    |<span data-ttu-id="c6818-111">説明</span><span class="sxs-lookup"><span data-stu-id="c6818-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6818-112">Get</span><span class="sxs-lookup"><span data-stu-id="c6818-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="c6818-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="c6818-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="c6818-114">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c6818-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="c6818-115">Add class</span><span class="sxs-lookup"><span data-stu-id="c6818-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="c6818-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="c6818-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="c6818-117">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="c6818-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="c6818-118">List classes</span><span class="sxs-lookup"><span data-stu-id="c6818-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="c6818-119">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c6818-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="c6818-120">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c6818-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="c6818-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="c6818-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="c6818-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="c6818-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="c6818-123">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="c6818-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="c6818-124">Add user</span><span class="sxs-lookup"><span data-stu-id="c6818-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="c6818-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="c6818-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c6818-126">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="c6818-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="c6818-127">List users</span><span class="sxs-lookup"><span data-stu-id="c6818-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="c6818-128">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c6818-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c6818-129">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c6818-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="c6818-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="c6818-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="c6818-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="c6818-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c6818-132">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="c6818-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="c6818-133">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c6818-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="c6818-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c6818-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="c6818-135">この **educationSchool** に対応する **administrativeUnit** を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6818-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="c6818-136">Update</span><span class="sxs-lookup"><span data-stu-id="c6818-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="c6818-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="c6818-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="c6818-138">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="c6818-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="c6818-139">Delete</span><span class="sxs-lookup"><span data-stu-id="c6818-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="c6818-140">なし</span><span class="sxs-lookup"><span data-stu-id="c6818-140">None</span></span> |<span data-ttu-id="c6818-141">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="c6818-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6818-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6818-142">Properties</span></span>
| <span data-ttu-id="c6818-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6818-143">Property</span></span>     | <span data-ttu-id="c6818-144">型</span><span class="sxs-lookup"><span data-stu-id="c6818-144">Type</span></span>   |<span data-ttu-id="c6818-145">説明</span><span class="sxs-lookup"><span data-stu-id="c6818-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6818-146">id</span><span class="sxs-lookup"><span data-stu-id="c6818-146">id</span></span>|<span data-ttu-id="c6818-147">文字列</span><span class="sxs-lookup"><span data-stu-id="c6818-147">String</span></span>|<span data-ttu-id="c6818-148">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="c6818-148">GUID of this school.</span></span>|
|<span data-ttu-id="c6818-149">displayName</span><span class="sxs-lookup"><span data-stu-id="c6818-149">displayName</span></span>| <span data-ttu-id="c6818-150">String</span><span class="sxs-lookup"><span data-stu-id="c6818-150">String</span></span>| <span data-ttu-id="c6818-151">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="c6818-151">Display name of the school.</span></span>| 
|<span data-ttu-id="c6818-152">説明</span><span class="sxs-lookup"><span data-stu-id="c6818-152">description</span></span>| <span data-ttu-id="c6818-153">文字列</span><span class="sxs-lookup"><span data-stu-id="c6818-153">String</span></span> | <span data-ttu-id="c6818-154">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="c6818-154">Description of the school.</span></span>| 
|<span data-ttu-id="c6818-155">status</span><span class="sxs-lookup"><span data-stu-id="c6818-155">status</span></span>| <span data-ttu-id="c6818-156">string</span><span class="sxs-lookup"><span data-stu-id="c6818-156">string</span></span>| <span data-ttu-id="c6818-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c6818-157">Read-Only.</span></span> <span data-ttu-id="c6818-158">使用可能な値: `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="c6818-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="c6818-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="c6818-159">externalSource</span></span>| <span data-ttu-id="c6818-160">string</span><span class="sxs-lookup"><span data-stu-id="c6818-160">string</span></span>| <span data-ttu-id="c6818-161">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c6818-161">Read-Only.</span></span>  <span data-ttu-id="c6818-162">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c6818-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c6818-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="c6818-163">principalEmail</span></span>| <span data-ttu-id="c6818-164">String</span><span class="sxs-lookup"><span data-stu-id="c6818-164">String</span></span>| <span data-ttu-id="c6818-165">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="c6818-165">Email address of the principal.</span></span>|
|<span data-ttu-id="c6818-166">principalName</span><span class="sxs-lookup"><span data-stu-id="c6818-166">principalName</span></span>| <span data-ttu-id="c6818-167">String</span><span class="sxs-lookup"><span data-stu-id="c6818-167">String</span></span> | <span data-ttu-id="c6818-168">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="c6818-168">Name of the principal.</span></span>|
|<span data-ttu-id="c6818-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="c6818-169">externalPrincipalId</span></span>| <span data-ttu-id="c6818-170">String</span><span class="sxs-lookup"><span data-stu-id="c6818-170">String</span></span> | <span data-ttu-id="c6818-171">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="c6818-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="c6818-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="c6818-172">highestGrade</span></span>|<span data-ttu-id="c6818-173">String</span><span class="sxs-lookup"><span data-stu-id="c6818-173">String</span></span>| <span data-ttu-id="c6818-174">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="c6818-174">Highest grade taught.</span></span> |
|<span data-ttu-id="c6818-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="c6818-175">lowestGrade</span></span>|<span data-ttu-id="c6818-176">String</span><span class="sxs-lookup"><span data-stu-id="c6818-176">String</span></span>| <span data-ttu-id="c6818-177">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="c6818-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="c6818-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="c6818-178">schoolNumber</span></span>|<span data-ttu-id="c6818-179">String</span><span class="sxs-lookup"><span data-stu-id="c6818-179">String</span></span>| <span data-ttu-id="c6818-180">学校番号。</span><span class="sxs-lookup"><span data-stu-id="c6818-180">School Number.</span></span>|
|<span data-ttu-id="c6818-181">externalId</span><span class="sxs-lookup"><span data-stu-id="c6818-181">externalId</span></span>|<span data-ttu-id="c6818-182">String</span><span class="sxs-lookup"><span data-stu-id="c6818-182">String</span></span>| <span data-ttu-id="c6818-183">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="c6818-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="c6818-184">phone</span><span class="sxs-lookup"><span data-stu-id="c6818-184">phone</span></span>|<span data-ttu-id="c6818-185">String</span><span class="sxs-lookup"><span data-stu-id="c6818-185">String</span></span>| <span data-ttu-id="c6818-186">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="c6818-186">Phone number of school.</span></span> |
|<span data-ttu-id="c6818-187">fax</span><span class="sxs-lookup"><span data-stu-id="c6818-187">fax</span></span>|<span data-ttu-id="c6818-188">String</span><span class="sxs-lookup"><span data-stu-id="c6818-188">String</span></span>| <span data-ttu-id="c6818-189">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="c6818-189">Fax number of school.</span></span> |
|<span data-ttu-id="c6818-190">address</span><span class="sxs-lookup"><span data-stu-id="c6818-190">address</span></span>|[<span data-ttu-id="c6818-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6818-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="c6818-192">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="c6818-192">Address of the school.</span></span>|
|<span data-ttu-id="c6818-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="c6818-193">createdBy</span></span>|[<span data-ttu-id="c6818-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="c6818-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="c6818-195">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="c6818-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c6818-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6818-196">Relationships</span></span>
| <span data-ttu-id="c6818-197">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6818-197">Relationship</span></span> | <span data-ttu-id="c6818-198">型</span><span class="sxs-lookup"><span data-stu-id="c6818-198">Type</span></span>   |<span data-ttu-id="c6818-199">説明</span><span class="sxs-lookup"><span data-stu-id="c6818-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6818-200">classes</span><span class="sxs-lookup"><span data-stu-id="c6818-200">classes</span></span>|<span data-ttu-id="c6818-201">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c6818-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="c6818-202">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="c6818-202">Classes taught at the school.</span></span> <span data-ttu-id="c6818-203">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c6818-203">Nullable.</span></span>|
|<span data-ttu-id="c6818-204">users</span><span class="sxs-lookup"><span data-stu-id="c6818-204">users</span></span>|<span data-ttu-id="c6818-205">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c6818-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c6818-206">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="c6818-206">Users in the school.</span></span> <span data-ttu-id="c6818-207">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c6818-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6818-208">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6818-208">JSON representation</span></span>

<span data-ttu-id="c6818-209">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6818-209">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
