---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーに対して権限を持つ役割の割り当てを表します。 '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515119"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="7cfd9-103">privilegedRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7cfd9-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cfd9-104">特定のユーザーに対して権限を持つ役割の割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="7cfd9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="7cfd9-105">Methods</span></span>

| <span data-ttu-id="7cfd9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7cfd9-106">Method</span></span>           | <span data-ttu-id="7cfd9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7cfd9-107">Return Type</span></span>    |<span data-ttu-id="7cfd9-108">説明</span><span class="sxs-lookup"><span data-stu-id="7cfd9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7cfd9-109">PrivilegedRoleAssignment コレクションのリスト</span><span class="sxs-lookup"><span data-stu-id="7cfd9-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="7cfd9-110">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7cfd9-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="7cfd9-111">PrivilegedRoleAssignment オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="7cfd9-112">PrivilegedRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="7cfd9-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7cfd9-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="7cfd9-114">PrivilegedRoleAssignment オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="7cfd9-115">割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="7cfd9-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7cfd9-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="7cfd9-117">割り当てのコレクションへの投稿には、新しい割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="7cfd9-118">Delete</span><span class="sxs-lookup"><span data-stu-id="7cfd9-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="7cfd9-119">なし</span><span class="sxs-lookup"><span data-stu-id="7cfd9-119">None</span></span> |<span data-ttu-id="7cfd9-120">PrivilegedRoleAssignment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="7cfd9-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="7cfd9-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="7cfd9-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7cfd9-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="7cfd9-123">として永続的な役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="7cfd9-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="7cfd9-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="7cfd9-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7cfd9-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="7cfd9-126">対象となるように、役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="7cfd9-127">My</span><span class="sxs-lookup"><span data-stu-id="7cfd9-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="7cfd9-128">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7cfd9-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="7cfd9-129">現在のユーザーの特権を持つ役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="7cfd9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cfd9-130">Properties</span></span>
| <span data-ttu-id="7cfd9-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cfd9-131">Property</span></span>     | <span data-ttu-id="7cfd9-132">型</span><span class="sxs-lookup"><span data-stu-id="7cfd9-132">Type</span></span>   |<span data-ttu-id="7cfd9-133">説明</span><span class="sxs-lookup"><span data-stu-id="7cfd9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cfd9-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7cfd9-134">expirationDateTime</span></span>|<span data-ttu-id="7cfd9-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cfd9-135">dateTimeOffset</span></span>|<span data-ttu-id="7cfd9-136">一時的な特権を持つロールの割り当ては期限が切れた場合は、UTC 日時です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="7cfd9-137">永続的な役割の割り当ての値が null です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="7cfd9-138">id</span><span class="sxs-lookup"><span data-stu-id="7cfd9-138">id</span></span>|<span data-ttu-id="7cfd9-139">string</span><span class="sxs-lookup"><span data-stu-id="7cfd9-139">string</span></span>| <span data-ttu-id="7cfd9-140">特権を持つ役割の割り当ての一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="7cfd9-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-141">Read-only.</span></span> <span data-ttu-id="7cfd9-142">'UserId_roleId'、Azure AD ユーザーの id の GUID の文字列は、ユーザー Id、roleId は、Azure の管理者ロールの id の GUID の文字列の形式であります。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="7cfd9-143">isElevated</span><span class="sxs-lookup"><span data-stu-id="7cfd9-143">isElevated</span></span>|<span data-ttu-id="7cfd9-144">boolean</span><span class="sxs-lookup"><span data-stu-id="7cfd9-144">boolean</span></span>|<span data-ttu-id="7cfd9-145">**true の**ロールの割り当てが有効な場合です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="7cfd9-146">**false**役割の割り当てが無効になった場合。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="7cfd9-147">resultMessage</span><span class="sxs-lookup"><span data-stu-id="7cfd9-147">resultMessage</span></span>|<span data-ttu-id="7cfd9-148">string</span><span class="sxs-lookup"><span data-stu-id="7cfd9-148">string</span></span>|<span data-ttu-id="7cfd9-149">結果のメッセージがサービスによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-149">Result message set by the service.</span></span>|
|<span data-ttu-id="7cfd9-150">roleId</span><span class="sxs-lookup"><span data-stu-id="7cfd9-150">roleId</span></span>|<span data-ttu-id="7cfd9-151">string</span><span class="sxs-lookup"><span data-stu-id="7cfd9-151">string</span></span>|<span data-ttu-id="7cfd9-152">ロール識別子</span><span class="sxs-lookup"><span data-stu-id="7cfd9-152">Role identifier.</span></span> <span data-ttu-id="7cfd9-153">GUID の文字列形式。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-153">In GUID string format.</span></span>|
|<span data-ttu-id="7cfd9-154">userId</span><span class="sxs-lookup"><span data-stu-id="7cfd9-154">userId</span></span>|<span data-ttu-id="7cfd9-155">string</span><span class="sxs-lookup"><span data-stu-id="7cfd9-155">string</span></span>|<span data-ttu-id="7cfd9-156">ユーザーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-156">User identifier.</span></span> <span data-ttu-id="7cfd9-157">GUID の文字列形式。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cfd9-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cfd9-158">Relationships</span></span>
| <span data-ttu-id="7cfd9-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cfd9-159">Relationship</span></span> | <span data-ttu-id="7cfd9-160">型</span><span class="sxs-lookup"><span data-stu-id="7cfd9-160">Type</span></span>   |<span data-ttu-id="7cfd9-161">説明</span><span class="sxs-lookup"><span data-stu-id="7cfd9-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cfd9-162">roleInfo</span><span class="sxs-lookup"><span data-stu-id="7cfd9-162">roleInfo</span></span>|[<span data-ttu-id="7cfd9-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="7cfd9-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="7cfd9-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-164">Read-only.</span></span> <span data-ttu-id="7cfd9-165">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-165">Nullable.</span></span> <span data-ttu-id="7cfd9-166">関連付けられているロールの情報です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cfd9-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7cfd9-167">JSON representation</span></span>

<span data-ttu-id="7cfd9-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7cfd9-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
