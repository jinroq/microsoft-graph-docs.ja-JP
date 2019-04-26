---
title: educationClass リソース タイプ
description: '学校内のクラスを表します。 **educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。 学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。 Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: c5b145d12dd99293eef9c338ff840d5781c5ef3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562714"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="a6ae8-106">educationClass リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-106">educationClass resource type</span></span>

<span data-ttu-id="a6ae8-107">学校内のクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-107">Represents a class within a school.</span></span> <span data-ttu-id="a6ae8-108">**educationClass** リソースは Office 365 グループに相当し、同じ ID を共有します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="a6ae8-109">学生はクラスの通常のメンバーであり、教師は所有者であり適切な権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="a6ae8-110">Office の操作性が適切に機能するために、教師は、teachers コレクションと members コレクションの両方のメンバーになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="a6ae8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6ae8-111">Methods</span></span>

| <span data-ttu-id="a6ae8-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6ae8-112">Method</span></span>           | <span data-ttu-id="a6ae8-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a6ae8-113">Return Type</span></span>    |<span data-ttu-id="a6ae8-114">説明</span><span class="sxs-lookup"><span data-stu-id="a6ae8-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6ae8-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="a6ae8-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="a6ae8-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="a6ae8-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="a6ae8-117">**educationClass** オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="a6ae8-118">Add member</span><span class="sxs-lookup"><span data-stu-id="a6ae8-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="a6ae8-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="a6ae8-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a6ae8-120">members ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="a6ae8-121">List members</span><span class="sxs-lookup"><span data-stu-id="a6ae8-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="a6ae8-122">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ae8-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a6ae8-123">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="a6ae8-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="a6ae8-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="a6ae8-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="a6ae8-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a6ae8-126">members ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="a6ae8-127">List schools</span><span class="sxs-lookup"><span data-stu-id="a6ae8-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="a6ae8-128">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ae8-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="a6ae8-129">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="a6ae8-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="a6ae8-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="a6ae8-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="a6ae8-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a6ae8-132">teachers ナビゲーション プロパティに投稿することで、クラスの新しい **educationUser** を追加します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="a6ae8-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="a6ae8-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="a6ae8-134">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ae8-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a6ae8-135">クラスの教師一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="a6ae8-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="a6ae8-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="a6ae8-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="a6ae8-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a6ae8-138">teachers ナビゲーション プロパティによって、クラスから **educationUser** を削除します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="a6ae8-139">Get group</span><span class="sxs-lookup"><span data-stu-id="a6ae8-139">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="a6ae8-140">group</span><span class="sxs-lookup"><span data-stu-id="a6ae8-140">group</span></span>](group.md)| <span data-ttu-id="a6ae8-141">この **educationClass** に対応する Office 365 **group**を取得します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-141">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="a6ae8-142">Update</span><span class="sxs-lookup"><span data-stu-id="a6ae8-142">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="a6ae8-143">educationClass</span><span class="sxs-lookup"><span data-stu-id="a6ae8-143">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="a6ae8-144">**educationClass** オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-144">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="a6ae8-145">削除</span><span class="sxs-lookup"><span data-stu-id="a6ae8-145">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="a6ae8-146">なし</span><span class="sxs-lookup"><span data-stu-id="a6ae8-146">None</span></span> |<span data-ttu-id="a6ae8-147">**educationClass** オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-147">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a6ae8-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-148">Properties</span></span>
| <span data-ttu-id="a6ae8-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-149">Property</span></span>     | <span data-ttu-id="a6ae8-150">型</span><span class="sxs-lookup"><span data-stu-id="a6ae8-150">Type</span></span>   |<span data-ttu-id="a6ae8-151">説明</span><span class="sxs-lookup"><span data-stu-id="a6ae8-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6ae8-152">id</span><span class="sxs-lookup"><span data-stu-id="a6ae8-152">id</span></span>| <span data-ttu-id="a6ae8-153">String</span><span class="sxs-lookup"><span data-stu-id="a6ae8-153">String</span></span>| <span data-ttu-id="a6ae8-154">クラスの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-154">Unique identifier for the class.</span></span>|
|<span data-ttu-id="a6ae8-155">説明</span><span class="sxs-lookup"><span data-stu-id="a6ae8-155">description</span></span>|<span data-ttu-id="a6ae8-156">String</span><span class="sxs-lookup"><span data-stu-id="a6ae8-156">String</span></span>| <span data-ttu-id="a6ae8-157">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-157">Description of the class.</span></span>|
|<span data-ttu-id="a6ae8-158">displayName</span><span class="sxs-lookup"><span data-stu-id="a6ae8-158">displayName</span></span>|<span data-ttu-id="a6ae8-159">文字列</span><span class="sxs-lookup"><span data-stu-id="a6ae8-159">String</span></span>| <span data-ttu-id="a6ae8-160">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-160">Name of the class.</span></span>|
|<span data-ttu-id="a6ae8-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a6ae8-161">mailNickname</span></span>|<span data-ttu-id="a6ae8-162">String</span><span class="sxs-lookup"><span data-stu-id="a6ae8-162">String</span></span>| <span data-ttu-id="a6ae8-163">すべてのメンバーに電子メールを送信する際のメール名 (この機能が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-163">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="a6ae8-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="a6ae8-164">createdBy</span></span>|[<span data-ttu-id="a6ae8-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="a6ae8-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="a6ae8-166">クラスを作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-166">Entity who created the class</span></span> |
|<span data-ttu-id="a6ae8-167">classCode</span><span class="sxs-lookup"><span data-stu-id="a6ae8-167">classCode</span></span>|<span data-ttu-id="a6ae8-168">String</span><span class="sxs-lookup"><span data-stu-id="a6ae8-168">String</span></span>| <span data-ttu-id="a6ae8-169">クラスを識別するために学校が使用するクラス コード。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-169">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="a6ae8-170">externalId</span><span class="sxs-lookup"><span data-stu-id="a6ae8-170">externalId</span></span>|<span data-ttu-id="a6ae8-171">String</span><span class="sxs-lookup"><span data-stu-id="a6ae8-171">String</span></span>| <span data-ttu-id="a6ae8-172">同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-172">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="a6ae8-173">externalName</span><span class="sxs-lookup"><span data-stu-id="a6ae8-173">externalName</span></span>|<span data-ttu-id="a6ae8-174">String</span><span class="sxs-lookup"><span data-stu-id="a6ae8-174">String</span></span>|<span data-ttu-id="a6ae8-175">同期システムからのクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-175">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="a6ae8-176">externalSource</span><span class="sxs-lookup"><span data-stu-id="a6ae8-176">externalSource</span></span>|<span data-ttu-id="a6ae8-177">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="a6ae8-177">educationExternalSource</span></span>| <span data-ttu-id="a6ae8-178">このクラスの作成方法。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-178">How this class was created.</span></span> <span data-ttu-id="a6ae8-179">使用可能な値: `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-179">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a6ae8-180">term</span><span class="sxs-lookup"><span data-stu-id="a6ae8-180">term</span></span>|[<span data-ttu-id="a6ae8-181">educationTerm</span><span class="sxs-lookup"><span data-stu-id="a6ae8-181">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="a6ae8-182">このクラスの学期。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-182">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6ae8-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-183">Relationships</span></span>
| <span data-ttu-id="a6ae8-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-184">Relationship</span></span> | <span data-ttu-id="a6ae8-185">型</span><span class="sxs-lookup"><span data-stu-id="a6ae8-185">Type</span></span>   |<span data-ttu-id="a6ae8-186">説明</span><span class="sxs-lookup"><span data-stu-id="a6ae8-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6ae8-187">members</span><span class="sxs-lookup"><span data-stu-id="a6ae8-187">members</span></span>|<span data-ttu-id="a6ae8-188">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ae8-188">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="a6ae8-189">クラスのすべてのユーザー。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-189">All users in the class.</span></span> <span data-ttu-id="a6ae8-190">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-190">Nullable.</span></span>|
|<span data-ttu-id="a6ae8-191">schools</span><span class="sxs-lookup"><span data-stu-id="a6ae8-191">schools</span></span>|<span data-ttu-id="a6ae8-192">[educationSchool](../resources/educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ae8-192">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="a6ae8-193">このクラスに関連付けられているすべての学校。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-193">All schools that this class is associated with.</span></span> <span data-ttu-id="a6ae8-194">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-194">Nullable.</span></span>|
|<span data-ttu-id="a6ae8-195">teachers</span><span class="sxs-lookup"><span data-stu-id="a6ae8-195">teachers</span></span>|<span data-ttu-id="a6ae8-196">[educationUser](../resources/educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6ae8-196">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="a6ae8-197">このクラスのすべての教師。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-197">All teachers in the class.</span></span> <span data-ttu-id="a6ae8-198">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-198">Nullable.</span></span>|
|<span data-ttu-id="a6ae8-199">グループ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-199">group</span></span>|[<span data-ttu-id="a6ae8-200">グループ</span><span class="sxs-lookup"><span data-stu-id="a6ae8-200">group</span></span>](../resources/group.md)| <span data-ttu-id="a6ae8-201">このクラスに対応するディレクトリグループ。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-201">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6ae8-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6ae8-202">JSON representation</span></span>

<span data-ttu-id="a6ae8-203">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6ae8-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
