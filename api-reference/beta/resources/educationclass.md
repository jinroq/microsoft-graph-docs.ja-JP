---
title: educationClass リソース タイプ
description: 学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bc9fa375e3f22087fbf268933370d8a6222654e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006368"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="d5393-104">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="d5393-104">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5393-105">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="d5393-105">Represents a class within a school.</span></span> <span data-ttu-id="d5393-106">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="d5393-106">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="d5393-107">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="d5393-107">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="d5393-108">Office 365 エクスペリエンスが正常に機能するには、教師が教師コレクションと members コレクションの両方のメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5393-108">For Office 365 experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

## <a name="methods"></a><span data-ttu-id="d5393-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d5393-109">Methods</span></span>

| <span data-ttu-id="d5393-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d5393-110">Method</span></span>                                                                  | <span data-ttu-id="d5393-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d5393-111">Return Type</span></span>                                    | <span data-ttu-id="d5393-112">説明</span><span class="sxs-lookup"><span data-stu-id="d5393-112">Description</span></span>                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [<span data-ttu-id="d5393-113">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="d5393-113">Get educationClass</span></span>](../api/educationclass-get.md)                      | <span data-ttu-id="d5393-114">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="d5393-114">[educationClass]</span></span>                               | <span data-ttu-id="d5393-115">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d5393-115">Read properties and relationships of an **educationClass** object.</span></span>                        |
| [<span data-ttu-id="d5393-116">Add member</span><span class="sxs-lookup"><span data-stu-id="d5393-116">Add member</span></span>](../api/educationclass-post-members.md)                     | <span data-ttu-id="d5393-117">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="d5393-117">[educationUser]</span></span>                                | <span data-ttu-id="d5393-118">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="d5393-118">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>  |
| [<span data-ttu-id="d5393-119">List members</span><span class="sxs-lookup"><span data-stu-id="d5393-119">List members</span></span>](../api/educationclass-list-members.md)                   | <span data-ttu-id="d5393-120">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-120">[educationUser] collection</span></span>                     | <span data-ttu-id="d5393-121">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d5393-121">Get an **educationUser** object collection.</span></span>                                               |
| [<span data-ttu-id="d5393-122">Remove student</span><span class="sxs-lookup"><span data-stu-id="d5393-122">Remove student</span></span>](../api/educationclass-delete-members.md)               | <span data-ttu-id="d5393-123">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="d5393-123">[educationUser]</span></span>                                | <span data-ttu-id="d5393-124">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="d5393-124">Remove an **educationUser** from the class through the members navigation property.</span></span>       |
| [<span data-ttu-id="d5393-125">List schools</span><span class="sxs-lookup"><span data-stu-id="d5393-125">List schools</span></span>](../api/educationclass-list-schools.md)                   | <span data-ttu-id="d5393-126">[educationSchool] コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-126">[educationSchool] collection</span></span>                   | <span data-ttu-id="d5393-127">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d5393-127">Get an **educationSchool** object collection.</span></span>                                             |
| [<span data-ttu-id="d5393-128">Add teacher</span><span class="sxs-lookup"><span data-stu-id="d5393-128">Add teacher</span></span>](../api/educationclass-post-teachers.md)                   | <span data-ttu-id="d5393-129">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="d5393-129">[educationUser]</span></span>                                | <span data-ttu-id="d5393-130">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="d5393-130">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span> |
| [<span data-ttu-id="d5393-131">List teachers</span><span class="sxs-lookup"><span data-stu-id="d5393-131">List teachers</span></span>](../api/educationclass-list-teachers.md)                 | <span data-ttu-id="d5393-132">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-132">[educationUser] collection</span></span>                     | <span data-ttu-id="d5393-133">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="d5393-133">Get a list of teachers for the class.</span></span>                                                     |
| [<span data-ttu-id="d5393-134">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="d5393-134">Remove teacher</span></span>](../api/educationclass-delete-teachers.md)              | <span data-ttu-id="d5393-135">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="d5393-135">[educationUser]</span></span>                                | <span data-ttu-id="d5393-136">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="d5393-136">Remove an **educationUser** from the class through the teachers navigation property.</span></span>      |
| [<span data-ttu-id="d5393-137">EducationAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="d5393-137">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) | <span data-ttu-id="d5393-138">[educationAssignment]</span><span class="sxs-lookup"><span data-stu-id="d5393-138">[educationAssignment]</span></span>                          | <span data-ttu-id="d5393-139">Assignments コレクションへの投稿によって新しい**educationAssignment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5393-139">Create a new **educationAssignment** by posting to the assignments collection.</span></span>            |
| [<span data-ttu-id="d5393-140">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d5393-140">List assignments</span></span>](../api/educationclass-list-assignments.md)           | <span data-ttu-id="d5393-141">[educationAssignment]コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-141">[educationAssignment]collection</span></span>                | <span data-ttu-id="d5393-142">**EducationAssignment**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d5393-142">Get an **educationAssignment** object collection.</span></span>                                         |
| [<span data-ttu-id="d5393-143">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="d5393-143">Get group</span></span>](../api/educationclass-get-group.md)                         | <span data-ttu-id="d5393-144">[group]</span><span class="sxs-lookup"><span data-stu-id="d5393-144">[group]</span></span>                                        | <span data-ttu-id="d5393-145">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="d5393-145">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>                 |
| [<span data-ttu-id="d5393-146">EducationCategory を作成する</span><span class="sxs-lookup"><span data-stu-id="d5393-146">Create educationCategory</span></span>](../api/educationclass-post-category.md)      | <span data-ttu-id="d5393-147">[educationCategory]</span><span class="sxs-lookup"><span data-stu-id="d5393-147">[educationCategory]</span></span>                            | <span data-ttu-id="d5393-148">このクラスの新しい**educationCategory**を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5393-148">Create a new **educationCategory** for this class.</span></span>                                        |
| [<span data-ttu-id="d5393-149">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="d5393-149">List categories</span></span>](../api/educationclass-list-categories.md)             | <span data-ttu-id="d5393-150">[educationCategory]コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-150">[educationCategory] collection</span></span>                 | <span data-ttu-id="d5393-151">このクラスに属する**educationCategory**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="d5393-151">Get a list of **educationCategory** objects belonging to this class.</span></span>                      |
| [<span data-ttu-id="d5393-152">Update</span><span class="sxs-lookup"><span data-stu-id="d5393-152">Update</span></span>](../api/educationclass-update.md)                               | <span data-ttu-id="d5393-153">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="d5393-153">[educationClass]</span></span>                               | <span data-ttu-id="d5393-154">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5393-154">Update **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="d5393-155">Delete</span><span class="sxs-lookup"><span data-stu-id="d5393-155">Delete</span></span>](../api/educationclass-delete.md)                               | <span data-ttu-id="d5393-156">None</span><span class="sxs-lookup"><span data-stu-id="d5393-156">None</span></span>                                           | <span data-ttu-id="d5393-157">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d5393-157">Delete **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="d5393-158">差分</span><span class="sxs-lookup"><span data-stu-id="d5393-158">Delta</span></span>](../api/educationclass-delta.md)                                 | <span data-ttu-id="d5393-159">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-159">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="d5393-160">**EducationClasses**の増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="d5393-160">Get incremental changes for **educationClasses**</span></span>                                          |

## <a name="properties"></a><span data-ttu-id="d5393-161">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5393-161">Properties</span></span>

| <span data-ttu-id="d5393-162">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5393-162">Property</span></span>       | <span data-ttu-id="d5393-163">型</span><span class="sxs-lookup"><span data-stu-id="d5393-163">Type</span></span>                                  | <span data-ttu-id="d5393-164">説明</span><span class="sxs-lookup"><span data-stu-id="d5393-164">Description</span></span>                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="d5393-165">id</span><span class="sxs-lookup"><span data-stu-id="d5393-165">id</span></span>             | <span data-ttu-id="d5393-166">文字列</span><span class="sxs-lookup"><span data-stu-id="d5393-166">String</span></span>                                | <span data-ttu-id="d5393-167">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="d5393-167">Unique identifier for the class.</span></span>                                                        |
| <span data-ttu-id="d5393-168">classCode</span><span class="sxs-lookup"><span data-stu-id="d5393-168">classCode</span></span>      | <span data-ttu-id="d5393-169">String</span><span class="sxs-lookup"><span data-stu-id="d5393-169">String</span></span>                                | <span data-ttu-id="d5393-170">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="d5393-170">Class code used by the school to identify the class.</span></span>                                    |
| <span data-ttu-id="d5393-171">学習</span><span class="sxs-lookup"><span data-stu-id="d5393-171">course</span></span>         | [<span data-ttu-id="d5393-172">educationCourse</span><span class="sxs-lookup"><span data-stu-id="d5393-172">educationCourse</span></span>](educationcourse.md) | <span data-ttu-id="d5393-173">クラスのコース情報</span><span class="sxs-lookup"><span data-stu-id="d5393-173">Course information for the class</span></span>                                                        |
| <span data-ttu-id="d5393-174">createdBy</span><span class="sxs-lookup"><span data-stu-id="d5393-174">createdBy</span></span>      | <span data-ttu-id="d5393-175">[identitySet]</span><span class="sxs-lookup"><span data-stu-id="d5393-175">[identitySet]</span></span>                         | <span data-ttu-id="d5393-176">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="d5393-176">Entity who created the class</span></span>                                                            |
| <span data-ttu-id="d5393-177">description</span><span class="sxs-lookup"><span data-stu-id="d5393-177">description</span></span>    | <span data-ttu-id="d5393-178">String</span><span class="sxs-lookup"><span data-stu-id="d5393-178">String</span></span>                                | <span data-ttu-id="d5393-179">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="d5393-179">Description of the class.</span></span>                                                               |
| <span data-ttu-id="d5393-180">displayName</span><span class="sxs-lookup"><span data-stu-id="d5393-180">displayName</span></span>    | <span data-ttu-id="d5393-181">文字列</span><span class="sxs-lookup"><span data-stu-id="d5393-181">String</span></span>                                | <span data-ttu-id="d5393-182">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="d5393-182">Name of the class.</span></span>                                                                      |
| <span data-ttu-id="d5393-183">externalId</span><span class="sxs-lookup"><span data-stu-id="d5393-183">externalId</span></span>     | <span data-ttu-id="d5393-184">String</span><span class="sxs-lookup"><span data-stu-id="d5393-184">String</span></span>                                | <span data-ttu-id="d5393-185">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="d5393-185">ID of the class from the syncing system.</span></span>                                                |
| <span data-ttu-id="d5393-186">externalName</span><span class="sxs-lookup"><span data-stu-id="d5393-186">externalName</span></span>   | <span data-ttu-id="d5393-187">String</span><span class="sxs-lookup"><span data-stu-id="d5393-187">String</span></span>                                | <span data-ttu-id="d5393-188">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="d5393-188">Name of the class in the syncing system.</span></span>                                                |
| <span data-ttu-id="d5393-189">externalSource</span><span class="sxs-lookup"><span data-stu-id="d5393-189">externalSource</span></span> | <span data-ttu-id="d5393-190">string</span><span class="sxs-lookup"><span data-stu-id="d5393-190">string</span></span>                                | <span data-ttu-id="d5393-191">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="d5393-191">How this class was created.</span></span> <span data-ttu-id="d5393-192">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d5393-192">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="d5393-193">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d5393-193">mailNickname</span></span>   | <span data-ttu-id="d5393-194">String</span><span class="sxs-lookup"><span data-stu-id="d5393-194">String</span></span>                                | <span data-ttu-id="d5393-195">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="d5393-195">Mail name for sending email to all members, if this is enabled.</span></span>                         |
| <span data-ttu-id="d5393-196">term</span><span class="sxs-lookup"><span data-stu-id="d5393-196">term</span></span>           | <span data-ttu-id="d5393-197">[educationTerm]</span><span class="sxs-lookup"><span data-stu-id="d5393-197">[educationTerm]</span></span>                       | <span data-ttu-id="d5393-198">クラスの用語。</span><span class="sxs-lookup"><span data-stu-id="d5393-198">Term for the class.</span></span>                                                                     |

## <a name="relationships"></a><span data-ttu-id="d5393-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5393-199">Relationships</span></span>

| <span data-ttu-id="d5393-200">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5393-200">Relationship</span></span> | <span data-ttu-id="d5393-201">型</span><span class="sxs-lookup"><span data-stu-id="d5393-201">Type</span></span>                             | <span data-ttu-id="d5393-202">説明</span><span class="sxs-lookup"><span data-stu-id="d5393-202">Description</span></span>                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| <span data-ttu-id="d5393-203">assignments</span><span class="sxs-lookup"><span data-stu-id="d5393-203">assignments</span></span>  | <span data-ttu-id="d5393-204">[educationAssignment]コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-204">[educationAssignment] collection</span></span> | <span data-ttu-id="d5393-205">このクラスに関連付けられているすべての割り当て。</span><span class="sxs-lookup"><span data-stu-id="d5393-205">All assignments associated with this class.</span></span> <span data-ttu-id="d5393-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d5393-206">Nullable.</span></span>     |
| <span data-ttu-id="d5393-207">members</span><span class="sxs-lookup"><span data-stu-id="d5393-207">members</span></span>      | <span data-ttu-id="d5393-208">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-208">[educationUser] collection</span></span>       | <span data-ttu-id="d5393-209">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="d5393-209">All users in the class.</span></span> <span data-ttu-id="d5393-210">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d5393-210">Nullable.</span></span>                         |
| <span data-ttu-id="d5393-211">schools</span><span class="sxs-lookup"><span data-stu-id="d5393-211">schools</span></span>      | <span data-ttu-id="d5393-212">[educationSchool] コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-212">[educationSchool] collection</span></span>     | <span data-ttu-id="d5393-213">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="d5393-213">All schools that this class is associated with.</span></span> <span data-ttu-id="d5393-214">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d5393-214">Nullable.</span></span> |
| <span data-ttu-id="d5393-215">teachers</span><span class="sxs-lookup"><span data-stu-id="d5393-215">teachers</span></span>     | <span data-ttu-id="d5393-216">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="d5393-216">[educationUser] collection</span></span>       | <span data-ttu-id="d5393-217">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="d5393-217">All teachers in the class.</span></span> <span data-ttu-id="d5393-218">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d5393-218">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="d5393-219">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5393-219">JSON representation</span></span>

<span data-ttu-id="d5393-220">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5393-220">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "classCode": "String",
  "course": { "@odata.type": "microsoft.graph.educationCourse" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "id": "String (identifier)",
  "mailNickname": "String",
  "term": { "@odata.type": "microsoft.graph.educationTerm" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.educationClass",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationClass has documented navigation properties, but we thought it was a complex type!",
    "Resource educationClass has documented navigation properties, but we thought it was a complex type!"
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[identityset]: identityset.md
[group]: group.md
