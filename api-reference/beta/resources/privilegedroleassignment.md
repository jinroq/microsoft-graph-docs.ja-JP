---
title: privilegedRoleAssignment リソースの種類
description: '特定のユーザーに対して権限を持つ役割の割り当てを表します。 '
localization_priority: Normal
ms.openlocfilehash: ec6bc34ecd56839c764592ff298475e8648f300b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823318"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="49377-103">privilegedRoleAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49377-103">privilegedRoleAssignment resource type</span></span>

> <span data-ttu-id="49377-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49377-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49377-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49377-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49377-106">特定のユーザーに対して権限を持つ役割の割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="49377-106">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="49377-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="49377-107">Methods</span></span>

| <span data-ttu-id="49377-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="49377-108">Method</span></span>           | <span data-ttu-id="49377-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="49377-109">Return Type</span></span>    |<span data-ttu-id="49377-110">説明</span><span class="sxs-lookup"><span data-stu-id="49377-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49377-111">PrivilegedRoleAssignment コレクションのリスト</span><span class="sxs-lookup"><span data-stu-id="49377-111">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="49377-112">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49377-112">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="49377-113">PrivilegedRoleAssignment オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="49377-113">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="49377-114">PrivilegedRoleAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="49377-114">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="49377-115">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="49377-115">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="49377-116">PrivilegedRoleAssignment オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49377-116">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="49377-117">割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="49377-117">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="49377-118">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="49377-118">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="49377-119">割り当てのコレクションへの投稿には、新しい割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="49377-119">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="49377-120">Delete</span><span class="sxs-lookup"><span data-stu-id="49377-120">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="49377-121">なし</span><span class="sxs-lookup"><span data-stu-id="49377-121">None</span></span> |<span data-ttu-id="49377-122">PrivilegedRoleAssignment オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="49377-122">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="49377-123">makePermanent</span><span class="sxs-lookup"><span data-stu-id="49377-123">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="49377-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="49377-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="49377-125">として永続的な役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="49377-125">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="49377-126">makeEligible</span><span class="sxs-lookup"><span data-stu-id="49377-126">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="49377-127">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="49377-127">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="49377-128">対象となるように、役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="49377-128">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="49377-129">私の</span><span class="sxs-lookup"><span data-stu-id="49377-129">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="49377-130">[privilegedRoleAssignment](privilegedroleassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49377-130">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="49377-131">現在のユーザーの特権を持つ役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="49377-131">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="49377-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49377-132">Properties</span></span>
| <span data-ttu-id="49377-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49377-133">Property</span></span>     | <span data-ttu-id="49377-134">種類</span><span class="sxs-lookup"><span data-stu-id="49377-134">Type</span></span>   |<span data-ttu-id="49377-135">説明</span><span class="sxs-lookup"><span data-stu-id="49377-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49377-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="49377-136">expirationDateTime</span></span>|<span data-ttu-id="49377-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49377-137">dateTimeOffset</span></span>|<span data-ttu-id="49377-138">一時的な特権を持つロールの割り当ては期限が切れた場合は、UTC 日時です。</span><span class="sxs-lookup"><span data-stu-id="49377-138">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="49377-139">永続的な役割の割り当ての値が null です。</span><span class="sxs-lookup"><span data-stu-id="49377-139">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="49377-140">ID</span><span class="sxs-lookup"><span data-stu-id="49377-140">id</span></span>|<span data-ttu-id="49377-141">文字列</span><span class="sxs-lookup"><span data-stu-id="49377-141">string</span></span>| <span data-ttu-id="49377-142">特権を持つ役割の割り当ての一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="49377-142">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="49377-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="49377-143">Read-only.</span></span> <span data-ttu-id="49377-144">'UserId_roleId'、Azure AD ユーザーの id の GUID の文字列は、ユーザー Id、roleId は、Azure の管理者ロールの id の GUID の文字列の形式であります。</span><span class="sxs-lookup"><span data-stu-id="49377-144">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="49377-145">isElevated</span><span class="sxs-lookup"><span data-stu-id="49377-145">isElevated</span></span>|<span data-ttu-id="49377-146">ブール</span><span class="sxs-lookup"><span data-stu-id="49377-146">boolean</span></span>|<span data-ttu-id="49377-147">**true の**ロールの割り当てが有効な場合です。</span><span class="sxs-lookup"><span data-stu-id="49377-147">**true** if the role assignment is activated.</span></span> <span data-ttu-id="49377-148">**false**役割の割り当てが無効になった場合。</span><span class="sxs-lookup"><span data-stu-id="49377-148">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="49377-149">resultMessage</span><span class="sxs-lookup"><span data-stu-id="49377-149">resultMessage</span></span>|<span data-ttu-id="49377-150">文字列</span><span class="sxs-lookup"><span data-stu-id="49377-150">string</span></span>|<span data-ttu-id="49377-151">結果のメッセージがサービスによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="49377-151">Result message set by the service.</span></span>|
|<span data-ttu-id="49377-152">roleId</span><span class="sxs-lookup"><span data-stu-id="49377-152">roleId</span></span>|<span data-ttu-id="49377-153">文字列</span><span class="sxs-lookup"><span data-stu-id="49377-153">string</span></span>|<span data-ttu-id="49377-154">ロールの識別子です。</span><span class="sxs-lookup"><span data-stu-id="49377-154">Role identifier.</span></span> <span data-ttu-id="49377-155">GUID の文字列形式。</span><span class="sxs-lookup"><span data-stu-id="49377-155">In GUID string format.</span></span>|
|<span data-ttu-id="49377-156">userId</span><span class="sxs-lookup"><span data-stu-id="49377-156">userId</span></span>|<span data-ttu-id="49377-157">文字列</span><span class="sxs-lookup"><span data-stu-id="49377-157">string</span></span>|<span data-ttu-id="49377-158">ユーザーの識別子です。</span><span class="sxs-lookup"><span data-stu-id="49377-158">User identifier.</span></span> <span data-ttu-id="49377-159">GUID の文字列形式。</span><span class="sxs-lookup"><span data-stu-id="49377-159">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49377-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49377-160">Relationships</span></span>
| <span data-ttu-id="49377-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49377-161">Relationship</span></span> | <span data-ttu-id="49377-162">型</span><span class="sxs-lookup"><span data-stu-id="49377-162">Type</span></span>   |<span data-ttu-id="49377-163">説明</span><span class="sxs-lookup"><span data-stu-id="49377-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49377-164">roleInfo</span><span class="sxs-lookup"><span data-stu-id="49377-164">roleInfo</span></span>|[<span data-ttu-id="49377-165">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="49377-165">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="49377-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="49377-166">Read-only.</span></span> <span data-ttu-id="49377-167">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="49377-167">Nullable.</span></span> <span data-ttu-id="49377-168">関連付けられているロールの情報です。</span><span class="sxs-lookup"><span data-stu-id="49377-168">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49377-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49377-169">JSON representation</span></span>

<span data-ttu-id="49377-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49377-170">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
