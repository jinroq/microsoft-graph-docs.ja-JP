---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーの特権の役割の割り当てを表します。 '
localization_priority: Normal
ms.openlocfilehash: 479b6d46dc479134fd0abb46b1a9ffe478611a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563425"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="474e4-103">privilegedRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="474e4-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="474e4-104">特定のユーザーの特権の役割の割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="474e4-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="474e4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="474e4-105">Methods</span></span>

| <span data-ttu-id="474e4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="474e4-106">Method</span></span>           | <span data-ttu-id="474e4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="474e4-107">Return Type</span></span>    |<span data-ttu-id="474e4-108">説明</span><span class="sxs-lookup"><span data-stu-id="474e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="474e4-109">privilegedRoleAssignment コレクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="474e4-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="474e4-110">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="474e4-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="474e4-111">privilegedRoleAssignment オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="474e4-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="474e4-112">privilegedRoleAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="474e4-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="474e4-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="474e4-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="474e4-114">privilegedRoleAssignment オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="474e4-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="474e4-115">割り当てを作成する</span><span class="sxs-lookup"><span data-stu-id="474e4-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="474e4-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="474e4-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="474e4-117">assignments コレクションに投稿して、新しい割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="474e4-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="474e4-118">削除</span><span class="sxs-lookup"><span data-stu-id="474e4-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="474e4-119">なし</span><span class="sxs-lookup"><span data-stu-id="474e4-119">None</span></span> |<span data-ttu-id="474e4-120">privilegedRoleAssignment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="474e4-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="474e4-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="474e4-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="474e4-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="474e4-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="474e4-123">役割の割り当てを永続的に設定します。</span><span class="sxs-lookup"><span data-stu-id="474e4-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="474e4-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="474e4-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="474e4-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="474e4-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="474e4-126">役割の割り当てを対象として設定します。</span><span class="sxs-lookup"><span data-stu-id="474e4-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="474e4-127">私の</span><span class="sxs-lookup"><span data-stu-id="474e4-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="474e4-128">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="474e4-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="474e4-129">現在のユーザーの特権の役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="474e4-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="474e4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="474e4-130">Properties</span></span>
| <span data-ttu-id="474e4-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="474e4-131">Property</span></span>     | <span data-ttu-id="474e4-132">型</span><span class="sxs-lookup"><span data-stu-id="474e4-132">Type</span></span>   |<span data-ttu-id="474e4-133">説明</span><span class="sxs-lookup"><span data-stu-id="474e4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="474e4-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="474e4-134">expirationDateTime</span></span>|<span data-ttu-id="474e4-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474e4-135">dateTimeOffset</span></span>|<span data-ttu-id="474e4-136">一時的な特権の役割の割り当てが期限切れになる UTC の DateTime。</span><span class="sxs-lookup"><span data-stu-id="474e4-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="474e4-137">永続的な役割の割り当ての場合、値は null になります。</span><span class="sxs-lookup"><span data-stu-id="474e4-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="474e4-138">id</span><span class="sxs-lookup"><span data-stu-id="474e4-138">id</span></span>|<span data-ttu-id="474e4-139">string</span><span class="sxs-lookup"><span data-stu-id="474e4-139">string</span></span>| <span data-ttu-id="474e4-140">特権の役割の割り当ての一意識別子。</span><span class="sxs-lookup"><span data-stu-id="474e4-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="474e4-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="474e4-141">Read-only.</span></span> <span data-ttu-id="474e4-142">これは ' userId_roleId ' の形式になっています。ここで、userId は azure AD ユーザー id の guid 文字列で、roleId は azure 管理者の役割 id の guid 文字列です。</span><span class="sxs-lookup"><span data-stu-id="474e4-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="474e4-143">isElevated</span><span class="sxs-lookup"><span data-stu-id="474e4-143">isElevated</span></span>|<span data-ttu-id="474e4-144">ブール値</span><span class="sxs-lookup"><span data-stu-id="474e4-144">boolean</span></span>|<span data-ttu-id="474e4-145">役割の割り当てがアクティブ化されている場合は**true** 。</span><span class="sxs-lookup"><span data-stu-id="474e4-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="474e4-146">**false**を指定すると、役割の割り当てが非アクティブになります。</span><span class="sxs-lookup"><span data-stu-id="474e4-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="474e4-147">resultmessage</span><span class="sxs-lookup"><span data-stu-id="474e4-147">resultMessage</span></span>|<span data-ttu-id="474e4-148">string</span><span class="sxs-lookup"><span data-stu-id="474e4-148">string</span></span>|<span data-ttu-id="474e4-149">サービスによって設定された結果メッセージ。</span><span class="sxs-lookup"><span data-stu-id="474e4-149">Result message set by the service.</span></span>|
|<span data-ttu-id="474e4-150">roleId</span><span class="sxs-lookup"><span data-stu-id="474e4-150">roleId</span></span>|<span data-ttu-id="474e4-151">string</span><span class="sxs-lookup"><span data-stu-id="474e4-151">string</span></span>|<span data-ttu-id="474e4-152">ロール識別子。</span><span class="sxs-lookup"><span data-stu-id="474e4-152">Role identifier.</span></span> <span data-ttu-id="474e4-153">GUID 文字列形式。</span><span class="sxs-lookup"><span data-stu-id="474e4-153">In GUID string format.</span></span>|
|<span data-ttu-id="474e4-154">userId</span><span class="sxs-lookup"><span data-stu-id="474e4-154">userId</span></span>|<span data-ttu-id="474e4-155">string</span><span class="sxs-lookup"><span data-stu-id="474e4-155">string</span></span>|<span data-ttu-id="474e4-156">ユーザー識別子。</span><span class="sxs-lookup"><span data-stu-id="474e4-156">User identifier.</span></span> <span data-ttu-id="474e4-157">GUID 文字列形式。</span><span class="sxs-lookup"><span data-stu-id="474e4-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="474e4-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="474e4-158">Relationships</span></span>
| <span data-ttu-id="474e4-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="474e4-159">Relationship</span></span> | <span data-ttu-id="474e4-160">型</span><span class="sxs-lookup"><span data-stu-id="474e4-160">Type</span></span>   |<span data-ttu-id="474e4-161">説明</span><span class="sxs-lookup"><span data-stu-id="474e4-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="474e4-162">roleinfo</span><span class="sxs-lookup"><span data-stu-id="474e4-162">roleInfo</span></span>|[<span data-ttu-id="474e4-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="474e4-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="474e4-164">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="474e4-164">Read-only.</span></span> <span data-ttu-id="474e4-165">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="474e4-165">Nullable.</span></span> <span data-ttu-id="474e4-166">関連付けられているロール情報。</span><span class="sxs-lookup"><span data-stu-id="474e4-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="474e4-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="474e4-167">JSON representation</span></span>

<span data-ttu-id="474e4-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="474e4-168">Here is a JSON representation of the resource.</span></span>

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
