---
title: educationClass リソース タイプ
description: 学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8a228c329427ae6b3f8da1a971817e88284be917
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750081"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="5aa91-104">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="5aa91-104">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aa91-105">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-105">Represents a class within a school.</span></span> <span data-ttu-id="5aa91-106">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-106">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="5aa91-107">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="5aa91-107">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="5aa91-108">Office 365 エクスペリエンスが正常に機能するには、教師が教師コレクションと members コレクションの両方のメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="5aa91-108">For Office 365 experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

## <a name="methods"></a><span data-ttu-id="5aa91-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5aa91-109">Methods</span></span>

| <span data-ttu-id="5aa91-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="5aa91-110">Method</span></span>                                                                  | <span data-ttu-id="5aa91-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5aa91-111">Return Type</span></span>                                    | <span data-ttu-id="5aa91-112">説明</span><span class="sxs-lookup"><span data-stu-id="5aa91-112">Description</span></span>                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [<span data-ttu-id="5aa91-113">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="5aa91-113">Get educationClass</span></span>](../api/educationclass-get.md)                      | <span data-ttu-id="5aa91-114">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="5aa91-114">[educationClass]</span></span>                               | <span data-ttu-id="5aa91-115">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5aa91-115">Read properties and relationships of an **educationClass** object.</span></span>                        |
| [<span data-ttu-id="5aa91-116">Add member</span><span class="sxs-lookup"><span data-stu-id="5aa91-116">Add member</span></span>](../api/educationclass-post-members.md)                     | <span data-ttu-id="5aa91-117">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="5aa91-117">[educationUser]</span></span>                                | <span data-ttu-id="5aa91-118">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-118">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>  |
| [<span data-ttu-id="5aa91-119">List members</span><span class="sxs-lookup"><span data-stu-id="5aa91-119">List members</span></span>](../api/educationclass-list-members.md)                   | <span data-ttu-id="5aa91-120">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-120">[educationUser] collection</span></span>                     | <span data-ttu-id="5aa91-121">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-121">Get an **educationUser** object collection.</span></span>                                               |
| [<span data-ttu-id="5aa91-122">Remove student</span><span class="sxs-lookup"><span data-stu-id="5aa91-122">Remove student</span></span>](../api/educationclass-delete-members.md)               | <span data-ttu-id="5aa91-123">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="5aa91-123">[educationUser]</span></span>                                | <span data-ttu-id="5aa91-124">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-124">Remove an **educationUser** from the class through the members navigation property.</span></span>       |
| [<span data-ttu-id="5aa91-125">List schools</span><span class="sxs-lookup"><span data-stu-id="5aa91-125">List schools</span></span>](../api/educationclass-list-schools.md)                   | <span data-ttu-id="5aa91-126">[educationSchool] コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-126">[educationSchool] collection</span></span>                   | <span data-ttu-id="5aa91-127">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-127">Get an **educationSchool** object collection.</span></span>                                             |
| [<span data-ttu-id="5aa91-128">Add teacher</span><span class="sxs-lookup"><span data-stu-id="5aa91-128">Add teacher</span></span>](../api/educationclass-post-teachers.md)                   | <span data-ttu-id="5aa91-129">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="5aa91-129">[educationUser]</span></span>                                | <span data-ttu-id="5aa91-130">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-130">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span> |
| [<span data-ttu-id="5aa91-131">List teachers</span><span class="sxs-lookup"><span data-stu-id="5aa91-131">List teachers</span></span>](../api/educationclass-list-teachers.md)                 | <span data-ttu-id="5aa91-132">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-132">[educationUser] collection</span></span>                     | <span data-ttu-id="5aa91-133">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-133">Get a list of teachers for the class.</span></span>                                                     |
| [<span data-ttu-id="5aa91-134">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="5aa91-134">Remove teacher</span></span>](../api/educationclass-delete-teachers.md)              | <span data-ttu-id="5aa91-135">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="5aa91-135">[educationUser]</span></span>                                | <span data-ttu-id="5aa91-136">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-136">Remove an **educationUser** from the class through the teachers navigation property.</span></span>      |
| [<span data-ttu-id="5aa91-137">EducationAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="5aa91-137">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) | <span data-ttu-id="5aa91-138">[educationAssignment]</span><span class="sxs-lookup"><span data-stu-id="5aa91-138">[educationAssignment]</span></span>                          | <span data-ttu-id="5aa91-139">Assignments コレクションへの投稿によって新しい**educationAssignment**を作成します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-139">Create a new **educationAssignment** by posting to the assignments collection.</span></span>            |
| [<span data-ttu-id="5aa91-140">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5aa91-140">List assignments</span></span>](../api/educationclass-list-assignments.md)           | <span data-ttu-id="5aa91-141">[educationAssignment]コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-141">[educationAssignment]collection</span></span>                | <span data-ttu-id="5aa91-142">**EducationAssignment**オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-142">Get an **educationAssignment** object collection.</span></span>                                         |
| [<span data-ttu-id="5aa91-143">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="5aa91-143">Get group</span></span>](../api/educationclass-get-group.md)                         | <span data-ttu-id="5aa91-144">[group]</span><span class="sxs-lookup"><span data-stu-id="5aa91-144">[group]</span></span>                                        | <span data-ttu-id="5aa91-145">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-145">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>                 |
| [<span data-ttu-id="5aa91-146">EducationCategory を作成する</span><span class="sxs-lookup"><span data-stu-id="5aa91-146">Create educationCategory</span></span>](../api/educationclass-post-category.md)      | <span data-ttu-id="5aa91-147">[educationCategory]</span><span class="sxs-lookup"><span data-stu-id="5aa91-147">[educationCategory]</span></span>                            | <span data-ttu-id="5aa91-148">このクラスの新しい**educationCategory**を作成します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-148">Create a new **educationCategory** for this class.</span></span>                                        |
| [<span data-ttu-id="5aa91-149">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="5aa91-149">List categories</span></span>](../api/educationclass-list-categories.md)             | <span data-ttu-id="5aa91-150">[educationCategory]コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-150">[educationCategory] collection</span></span>                 | <span data-ttu-id="5aa91-151">このクラスに属する**educationCategory**オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-151">Get a list of **educationCategory** objects belonging to this class.</span></span>                      |
| [<span data-ttu-id="5aa91-152">Update</span><span class="sxs-lookup"><span data-stu-id="5aa91-152">Update</span></span>](../api/educationclass-update.md)                               | <span data-ttu-id="5aa91-153">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="5aa91-153">[educationClass]</span></span>                               | <span data-ttu-id="5aa91-154">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-154">Update **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="5aa91-155">Delete</span><span class="sxs-lookup"><span data-stu-id="5aa91-155">Delete</span></span>](../api/educationclass-delete.md)                               | <span data-ttu-id="5aa91-156">None</span><span class="sxs-lookup"><span data-stu-id="5aa91-156">None</span></span>                                           | <span data-ttu-id="5aa91-157">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-157">Delete **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="5aa91-158">差分</span><span class="sxs-lookup"><span data-stu-id="5aa91-158">Delta</span></span>](../api/educationclass-delta.md)                                 | <span data-ttu-id="5aa91-159">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-159">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="5aa91-160">**EducationClasses**の増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="5aa91-160">Get incremental changes for **educationClasses**</span></span>                                          |

## <a name="properties"></a><span data-ttu-id="5aa91-161">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5aa91-161">Properties</span></span>

| <span data-ttu-id="5aa91-162">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5aa91-162">Property</span></span>       | <span data-ttu-id="5aa91-163">型</span><span class="sxs-lookup"><span data-stu-id="5aa91-163">Type</span></span>                                  | <span data-ttu-id="5aa91-164">説明</span><span class="sxs-lookup"><span data-stu-id="5aa91-164">Description</span></span>                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="5aa91-165">id</span><span class="sxs-lookup"><span data-stu-id="5aa91-165">id</span></span>             | <span data-ttu-id="5aa91-166">文字列</span><span class="sxs-lookup"><span data-stu-id="5aa91-166">String</span></span>                                | <span data-ttu-id="5aa91-167">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5aa91-167">Unique identifier for the class.</span></span>                                                        |
| <span data-ttu-id="5aa91-168">classCode</span><span class="sxs-lookup"><span data-stu-id="5aa91-168">classCode</span></span>      | <span data-ttu-id="5aa91-169">String</span><span class="sxs-lookup"><span data-stu-id="5aa91-169">String</span></span>                                | <span data-ttu-id="5aa91-170">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="5aa91-170">Class code used by the school to identify the class.</span></span>                                    |
| <span data-ttu-id="5aa91-171">学習</span><span class="sxs-lookup"><span data-stu-id="5aa91-171">course</span></span>         | [<span data-ttu-id="5aa91-172">educationCourse</span><span class="sxs-lookup"><span data-stu-id="5aa91-172">educationCourse</span></span>](educationcourse.md) | <span data-ttu-id="5aa91-173">クラスのコース情報</span><span class="sxs-lookup"><span data-stu-id="5aa91-173">Course information for the class</span></span>                                                        |
| <span data-ttu-id="5aa91-174">createdBy</span><span class="sxs-lookup"><span data-stu-id="5aa91-174">createdBy</span></span>      | <span data-ttu-id="5aa91-175">[identitySet]</span><span class="sxs-lookup"><span data-stu-id="5aa91-175">[identitySet]</span></span>                         | <span data-ttu-id="5aa91-176">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="5aa91-176">Entity who created the class</span></span>                                                            |
| <span data-ttu-id="5aa91-177">description</span><span class="sxs-lookup"><span data-stu-id="5aa91-177">description</span></span>    | <span data-ttu-id="5aa91-178">String</span><span class="sxs-lookup"><span data-stu-id="5aa91-178">String</span></span>                                | <span data-ttu-id="5aa91-179">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="5aa91-179">Description of the class.</span></span>                                                               |
| <span data-ttu-id="5aa91-180">displayName</span><span class="sxs-lookup"><span data-stu-id="5aa91-180">displayName</span></span>    | <span data-ttu-id="5aa91-181">文字列</span><span class="sxs-lookup"><span data-stu-id="5aa91-181">String</span></span>                                | <span data-ttu-id="5aa91-182">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="5aa91-182">Name of the class.</span></span>                                                                      |
| <span data-ttu-id="5aa91-183">externalId</span><span class="sxs-lookup"><span data-stu-id="5aa91-183">externalId</span></span>     | <span data-ttu-id="5aa91-184">String</span><span class="sxs-lookup"><span data-stu-id="5aa91-184">String</span></span>                                | <span data-ttu-id="5aa91-185">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="5aa91-185">ID of the class from the syncing system.</span></span>                                                |
| <span data-ttu-id="5aa91-186">externalName</span><span class="sxs-lookup"><span data-stu-id="5aa91-186">externalName</span></span>   | <span data-ttu-id="5aa91-187">String</span><span class="sxs-lookup"><span data-stu-id="5aa91-187">String</span></span>                                | <span data-ttu-id="5aa91-188">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="5aa91-188">Name of the class in the syncing system.</span></span>                                                |
| <span data-ttu-id="5aa91-189">externalSource</span><span class="sxs-lookup"><span data-stu-id="5aa91-189">externalSource</span></span> | <span data-ttu-id="5aa91-190">string</span><span class="sxs-lookup"><span data-stu-id="5aa91-190">string</span></span>                                | <span data-ttu-id="5aa91-191">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="5aa91-191">How this class was created.</span></span> <span data-ttu-id="5aa91-192">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5aa91-192">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="5aa91-193">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5aa91-193">mailNickname</span></span>   | <span data-ttu-id="5aa91-194">String</span><span class="sxs-lookup"><span data-stu-id="5aa91-194">String</span></span>                                | <span data-ttu-id="5aa91-195">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="5aa91-195">Mail name for sending email to all members, if this is enabled.</span></span>                         |
| <span data-ttu-id="5aa91-196">term</span><span class="sxs-lookup"><span data-stu-id="5aa91-196">term</span></span>           | <span data-ttu-id="5aa91-197">[educationTerm]</span><span class="sxs-lookup"><span data-stu-id="5aa91-197">[educationTerm]</span></span>                       | <span data-ttu-id="5aa91-198">クラスの用語。</span><span class="sxs-lookup"><span data-stu-id="5aa91-198">Term for the class.</span></span>                                                                     |

## <a name="relationships"></a><span data-ttu-id="5aa91-199">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5aa91-199">Relationships</span></span>

| <span data-ttu-id="5aa91-200">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5aa91-200">Relationship</span></span> | <span data-ttu-id="5aa91-201">型</span><span class="sxs-lookup"><span data-stu-id="5aa91-201">Type</span></span>                             | <span data-ttu-id="5aa91-202">説明</span><span class="sxs-lookup"><span data-stu-id="5aa91-202">Description</span></span>                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| <span data-ttu-id="5aa91-203">assignments</span><span class="sxs-lookup"><span data-stu-id="5aa91-203">assignments</span></span>  | <span data-ttu-id="5aa91-204">[educationAssignment]コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-204">[educationAssignment] collection</span></span> | <span data-ttu-id="5aa91-205">このクラスに関連付けられているすべての割り当て。</span><span class="sxs-lookup"><span data-stu-id="5aa91-205">All assignments associated with this class.</span></span> <span data-ttu-id="5aa91-206">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5aa91-206">Nullable.</span></span>     |
| <span data-ttu-id="5aa91-207">members</span><span class="sxs-lookup"><span data-stu-id="5aa91-207">members</span></span>      | <span data-ttu-id="5aa91-208">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-208">[educationUser] collection</span></span>       | <span data-ttu-id="5aa91-209">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="5aa91-209">All users in the class.</span></span> <span data-ttu-id="5aa91-210">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5aa91-210">Nullable.</span></span>                         |
| <span data-ttu-id="5aa91-211">schools</span><span class="sxs-lookup"><span data-stu-id="5aa91-211">schools</span></span>      | <span data-ttu-id="5aa91-212">[educationSchool] コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-212">[educationSchool] collection</span></span>     | <span data-ttu-id="5aa91-213">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="5aa91-213">All schools that this class is associated with.</span></span> <span data-ttu-id="5aa91-214">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5aa91-214">Nullable.</span></span> |
| <span data-ttu-id="5aa91-215">teachers</span><span class="sxs-lookup"><span data-stu-id="5aa91-215">teachers</span></span>     | <span data-ttu-id="5aa91-216">[educationUser] コレクション</span><span class="sxs-lookup"><span data-stu-id="5aa91-216">[educationUser] collection</span></span>       | <span data-ttu-id="5aa91-217">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="5aa91-217">All teachers in the class.</span></span> <span data-ttu-id="5aa91-218">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="5aa91-218">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="5aa91-219">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5aa91-219">JSON representation</span></span>

<span data-ttu-id="5aa91-220">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5aa91-220">The following is a JSON representation of the resource.</span></span>

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
