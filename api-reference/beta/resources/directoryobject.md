---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
ms.openlocfilehash: ed49c042ab9456479d0f9f7fee49a72a93767e81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073676"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="8991e-104">directoryObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8991e-104">directoryObject resource type</span></span>

> <span data-ttu-id="8991e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8991e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8991e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8991e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8991e-p103">Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。</span><span class="sxs-lookup"><span data-stu-id="8991e-p103">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="8991e-109">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="8991e-109">This resource supports:</span></span>

- <span data-ttu-id="8991e-110">[デルタ](../api/directoryobject-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="8991e-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="8991e-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="8991e-111">Methods</span></span>

| <span data-ttu-id="8991e-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="8991e-112">Method</span></span>       | <span data-ttu-id="8991e-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8991e-113">Return Type</span></span>  |<span data-ttu-id="8991e-114">説明</span><span class="sxs-lookup"><span data-stu-id="8991e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8991e-115">directoryObject を取得する</span><span class="sxs-lookup"><span data-stu-id="8991e-115">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="8991e-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8991e-116">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="8991e-117">ディレクトリ オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8991e-117">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="8991e-118">削除</span><span class="sxs-lookup"><span data-stu-id="8991e-118">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="8991e-119">なし</span><span class="sxs-lookup"><span data-stu-id="8991e-119">None</span></span> |<span data-ttu-id="8991e-120">ディレクトリ オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8991e-120">Delete a directory object.</span></span> |
|[<span data-ttu-id="8991e-121">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8991e-121">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="8991e-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8991e-122">String collection</span></span>|<span data-ttu-id="8991e-p104">グループの一覧内のメンバーシップを確認します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="8991e-p104">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="8991e-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8991e-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="8991e-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8991e-126">String collection</span></span>|<span data-ttu-id="8991e-p105">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="8991e-p105">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="8991e-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="8991e-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="8991e-130">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8991e-130">String collection</span></span>| <span data-ttu-id="8991e-p106">ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。</span><span class="sxs-lookup"><span data-stu-id="8991e-p106">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="8991e-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="8991e-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="8991e-134">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8991e-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="8991e-135">指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="8991e-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="8991e-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="8991e-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="8991e-137">JSON</span><span class="sxs-lookup"><span data-stu-id="8991e-137">JSON</span></span>| <span data-ttu-id="8991e-138">メールのニックネームは、命名ポリシーに準拠しているまたは、Office 365 のグループの表示名を検証します。</span><span class="sxs-lookup"><span data-stu-id="8991e-138">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="8991e-139">delta</span><span class="sxs-lookup"><span data-stu-id="8991e-139">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="8991e-140">directoryObject コレクション</span><span class="sxs-lookup"><span data-stu-id="8991e-140">directoryObject collection</span></span>| <span data-ttu-id="8991e-141">ディレクトリ オブジェクトに対して増分の変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="8991e-141">Get incremental changes for directory objects.</span></span> <span data-ttu-id="8991e-142">Derrived の種類でフィルター処理をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8991e-142">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="8991e-143">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8991e-143">Properties</span></span>

| <span data-ttu-id="8991e-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8991e-144">Property</span></span>   | <span data-ttu-id="8991e-145">型</span><span class="sxs-lookup"><span data-stu-id="8991e-145">Type</span></span> |<span data-ttu-id="8991e-146">説明</span><span class="sxs-lookup"><span data-stu-id="8991e-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8991e-147">id</span><span class="sxs-lookup"><span data-stu-id="8991e-147">id</span></span>|<span data-ttu-id="8991e-148">String</span><span class="sxs-lookup"><span data-stu-id="8991e-148">String</span></span>|<span data-ttu-id="8991e-149">オブジェクトの一意の識別子である Guidたとえば、12345678-9abc-def0-1234-56789abcde12 です。</span><span class="sxs-lookup"><span data-stu-id="8991e-149">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="8991e-150">キー。</span><span class="sxs-lookup"><span data-stu-id="8991e-150">Key.</span></span> <span data-ttu-id="8991e-151">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="8991e-151">Not nullable.</span></span> <span data-ttu-id="8991e-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8991e-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8991e-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8991e-153">Relationships</span></span>

<span data-ttu-id="8991e-154">なし</span><span class="sxs-lookup"><span data-stu-id="8991e-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8991e-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8991e-155">JSON representation</span></span>

<span data-ttu-id="8991e-156">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8991e-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
