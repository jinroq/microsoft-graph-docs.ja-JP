---
title: educationSchool リソースの種類
description: '学校。 **EducationSchool**リソースは現在、administrativeUnit リソースに対応しており、同じ ID を共有しています。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b5e0807ae73110a921c70beef6a98589db41269
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972552"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="586c0-104">educationSchool リソースの種類</span><span class="sxs-lookup"><span data-stu-id="586c0-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="586c0-105">学校。</span><span class="sxs-lookup"><span data-stu-id="586c0-105">A school.</span></span> <span data-ttu-id="586c0-106">**EducationSchool**リソースは現在、 [administrativeUnit](administrativeunit.md)リソースに対応しており、同じ ID を共有しています。</span><span class="sxs-lookup"><span data-stu-id="586c0-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="586c0-107">このリソースは[educationOrganization](educationorganization.md)のサブタイプです。</span><span class="sxs-lookup"><span data-stu-id="586c0-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="586c0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="586c0-108">Methods</span></span>

| <span data-ttu-id="586c0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="586c0-109">Method</span></span>                                                                     | <span data-ttu-id="586c0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="586c0-110">Return Type</span></span>                                      | <span data-ttu-id="586c0-111">説明</span><span class="sxs-lookup"><span data-stu-id="586c0-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="586c0-112">Get</span><span class="sxs-lookup"><span data-stu-id="586c0-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="586c0-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="586c0-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="586c0-114">**educationSchool** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="586c0-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="586c0-115">Add class</span><span class="sxs-lookup"><span data-stu-id="586c0-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="586c0-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="586c0-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="586c0-117">classes ナビゲーション プロパティに投稿することで、学校の新しい **educationClass** を追加します。</span><span class="sxs-lookup"><span data-stu-id="586c0-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="586c0-118">List classes</span><span class="sxs-lookup"><span data-stu-id="586c0-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="586c0-119">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="586c0-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="586c0-120">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="586c0-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="586c0-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="586c0-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="586c0-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="586c0-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="586c0-123">classes ナビゲーション プロパティによって、学校から **educationClass** を削除します。</span><span class="sxs-lookup"><span data-stu-id="586c0-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="586c0-124">Add user</span><span class="sxs-lookup"><span data-stu-id="586c0-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="586c0-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="586c0-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="586c0-126">**users** ナビゲーション プロパティを投稿することで、学校の新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="586c0-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="586c0-127">List users</span><span class="sxs-lookup"><span data-stu-id="586c0-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="586c0-128">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="586c0-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="586c0-129">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="586c0-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="586c0-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="586c0-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="586c0-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="586c0-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="586c0-132">**users** ナビゲーション プロパティによって、学校から **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="586c0-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="586c0-133">AdministrativeUnit を取得する</span><span class="sxs-lookup"><span data-stu-id="586c0-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="586c0-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="586c0-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="586c0-135">この**educationSchool**に対応する**administrativeUnit**を取得します。</span><span class="sxs-lookup"><span data-stu-id="586c0-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="586c0-136">Update</span><span class="sxs-lookup"><span data-stu-id="586c0-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="586c0-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="586c0-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="586c0-138">**educationSchool** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="586c0-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="586c0-139">Delete</span><span class="sxs-lookup"><span data-stu-id="586c0-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="586c0-140">None</span><span class="sxs-lookup"><span data-stu-id="586c0-140">None</span></span>                                             | <span data-ttu-id="586c0-141">**educationSchool** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="586c0-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="586c0-142">差分</span><span class="sxs-lookup"><span data-stu-id="586c0-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="586c0-143">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="586c0-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="586c0-144">**EducationSchools**の増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="586c0-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="586c0-145">プロパティ</span><span class="sxs-lookup"><span data-stu-id="586c0-145">Properties</span></span>

| <span data-ttu-id="586c0-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="586c0-146">Property</span></span>            | <span data-ttu-id="586c0-147">型</span><span class="sxs-lookup"><span data-stu-id="586c0-147">Type</span></span>                                  | <span data-ttu-id="586c0-148">説明</span><span class="sxs-lookup"><span data-stu-id="586c0-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="586c0-149">id</span><span class="sxs-lookup"><span data-stu-id="586c0-149">id</span></span>                  | <span data-ttu-id="586c0-150">文字列</span><span class="sxs-lookup"><span data-stu-id="586c0-150">String</span></span>                                | <span data-ttu-id="586c0-151">この学校の GUID。</span><span class="sxs-lookup"><span data-stu-id="586c0-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="586c0-152">address</span><span class="sxs-lookup"><span data-stu-id="586c0-152">address</span></span>             | [<span data-ttu-id="586c0-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="586c0-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="586c0-154">学校の住所。</span><span class="sxs-lookup"><span data-stu-id="586c0-154">Address of the school.</span></span>                             |
| <span data-ttu-id="586c0-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="586c0-155">createdBy</span></span>           | [<span data-ttu-id="586c0-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="586c0-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="586c0-157">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="586c0-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="586c0-158">description</span><span class="sxs-lookup"><span data-stu-id="586c0-158">description</span></span>         | <span data-ttu-id="586c0-159">String</span><span class="sxs-lookup"><span data-stu-id="586c0-159">String</span></span>                                | <span data-ttu-id="586c0-160">学校の説明。</span><span class="sxs-lookup"><span data-stu-id="586c0-160">Description of the school.</span></span>                         |
| <span data-ttu-id="586c0-161">displayName</span><span class="sxs-lookup"><span data-stu-id="586c0-161">displayName</span></span>         | <span data-ttu-id="586c0-162">String</span><span class="sxs-lookup"><span data-stu-id="586c0-162">String</span></span>                                | <span data-ttu-id="586c0-163">学校の表示名。</span><span class="sxs-lookup"><span data-stu-id="586c0-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="586c0-164">externalId</span><span class="sxs-lookup"><span data-stu-id="586c0-164">externalId</span></span>          | <span data-ttu-id="586c0-165">String</span><span class="sxs-lookup"><span data-stu-id="586c0-165">String</span></span>                                | <span data-ttu-id="586c0-166">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="586c0-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="586c0-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="586c0-167">externalPrincipalId</span></span> | <span data-ttu-id="586c0-168">String</span><span class="sxs-lookup"><span data-stu-id="586c0-168">String</span></span>                                | <span data-ttu-id="586c0-169">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="586c0-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="586c0-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="586c0-170">externalSource</span></span>      | <span data-ttu-id="586c0-171">string</span><span class="sxs-lookup"><span data-stu-id="586c0-171">string</span></span>                                | <span data-ttu-id="586c0-172">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="586c0-172">Read-Only.</span></span> <span data-ttu-id="586c0-173">使用可能な値: `sis` または `manual`。</span><span class="sxs-lookup"><span data-stu-id="586c0-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="586c0-174">fax</span><span class="sxs-lookup"><span data-stu-id="586c0-174">fax</span></span>                 | <span data-ttu-id="586c0-175">String</span><span class="sxs-lookup"><span data-stu-id="586c0-175">String</span></span>                                | <span data-ttu-id="586c0-176">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="586c0-176">Fax number of school.</span></span>                              |
| <span data-ttu-id="586c0-177">highestGrade</span><span class="sxs-lookup"><span data-stu-id="586c0-177">highestGrade</span></span>        | <span data-ttu-id="586c0-178">String</span><span class="sxs-lookup"><span data-stu-id="586c0-178">String</span></span>                                | <span data-ttu-id="586c0-179">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="586c0-179">Highest grade taught.</span></span>                              |
| <span data-ttu-id="586c0-180">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="586c0-180">lowestGrade</span></span>         | <span data-ttu-id="586c0-181">String</span><span class="sxs-lookup"><span data-stu-id="586c0-181">String</span></span>                                | <span data-ttu-id="586c0-182">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="586c0-182">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="586c0-183">phone</span><span class="sxs-lookup"><span data-stu-id="586c0-183">phone</span></span>               | <span data-ttu-id="586c0-184">String</span><span class="sxs-lookup"><span data-stu-id="586c0-184">String</span></span>                                | <span data-ttu-id="586c0-185">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="586c0-185">Phone number of school.</span></span>                            |
| <span data-ttu-id="586c0-186">principalEmail</span><span class="sxs-lookup"><span data-stu-id="586c0-186">principalEmail</span></span>      | <span data-ttu-id="586c0-187">String</span><span class="sxs-lookup"><span data-stu-id="586c0-187">String</span></span>                                | <span data-ttu-id="586c0-188">プリンシパルの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="586c0-188">Email address of the principal.</span></span>                    |
| <span data-ttu-id="586c0-189">principalName</span><span class="sxs-lookup"><span data-stu-id="586c0-189">principalName</span></span>       | <span data-ttu-id="586c0-190">String</span><span class="sxs-lookup"><span data-stu-id="586c0-190">String</span></span>                                | <span data-ttu-id="586c0-191">プリンシパルの名前。</span><span class="sxs-lookup"><span data-stu-id="586c0-191">Name of the principal.</span></span>                             |
| <span data-ttu-id="586c0-192">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="586c0-192">schoolNumber</span></span>        | <span data-ttu-id="586c0-193">String</span><span class="sxs-lookup"><span data-stu-id="586c0-193">String</span></span>                                | <span data-ttu-id="586c0-194">学校番号。</span><span class="sxs-lookup"><span data-stu-id="586c0-194">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="586c0-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="586c0-195">Relationships</span></span>

| <span data-ttu-id="586c0-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="586c0-196">Relationship</span></span> | <span data-ttu-id="586c0-197">型</span><span class="sxs-lookup"><span data-stu-id="586c0-197">Type</span></span>                                           | <span data-ttu-id="586c0-198">説明</span><span class="sxs-lookup"><span data-stu-id="586c0-198">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="586c0-199">classes</span><span class="sxs-lookup"><span data-stu-id="586c0-199">classes</span></span>      | <span data-ttu-id="586c0-200">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="586c0-200">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="586c0-201">学校で授業しているクラス。</span><span class="sxs-lookup"><span data-stu-id="586c0-201">Classes taught at the school.</span></span> <span data-ttu-id="586c0-202">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="586c0-202">Nullable.</span></span> |
| <span data-ttu-id="586c0-203">users</span><span class="sxs-lookup"><span data-stu-id="586c0-203">users</span></span>        | <span data-ttu-id="586c0-204">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="586c0-204">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="586c0-205">学校のユーザー。</span><span class="sxs-lookup"><span data-stu-id="586c0-205">Users in the school.</span></span> <span data-ttu-id="586c0-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="586c0-206">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="586c0-207">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="586c0-207">JSON representation</span></span>

<span data-ttu-id="586c0-208">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="586c0-208">The following is a JSON representation of the resource.</span></span>

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->


```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "fax": "String",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationSchool has documented navigation properties, but we thought it was a complex type!" 
  ]  
}-->
