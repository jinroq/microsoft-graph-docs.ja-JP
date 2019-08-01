---
title: contactFolder リソース型
description: 連絡先が格納されたフォルダーです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 84ca2fff70adff1acdf63e62f19c64f18c7518c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029653"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="e8f90-103">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="e8f90-103">contactFolder resource type</span></span>

<span data-ttu-id="e8f90-104">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="e8f90-104">A folder that contains contacts.</span></span>

<span data-ttu-id="e8f90-105">このリソースでは、[デルタ](../api/contactfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="e8f90-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="e8f90-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8f90-106">Methods</span></span>

| <span data-ttu-id="e8f90-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8f90-107">Method</span></span>       | <span data-ttu-id="e8f90-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e8f90-108">Return Type</span></span>  |<span data-ttu-id="e8f90-109">説明</span><span class="sxs-lookup"><span data-stu-id="e8f90-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8f90-110">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="e8f90-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="e8f90-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="e8f90-112">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="e8f90-113">更新する</span><span class="sxs-lookup"><span data-stu-id="e8f90-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="e8f90-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="e8f90-115">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="e8f90-116">Delete</span><span class="sxs-lookup"><span data-stu-id="e8f90-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="e8f90-117">None</span><span class="sxs-lookup"><span data-stu-id="e8f90-117">None</span></span> |<span data-ttu-id="e8f90-118">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="e8f90-119">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e8f90-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="e8f90-120">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="e8f90-120">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="e8f90-121">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="e8f90-122">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="e8f90-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="e8f90-123">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-123">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="e8f90-124">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="e8f90-125">delta</span><span class="sxs-lookup"><span data-stu-id="e8f90-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="e8f90-126">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e8f90-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="e8f90-127">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="e8f90-128">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e8f90-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="e8f90-129">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="e8f90-129">[Contact](contact.md) collection</span></span>| <span data-ttu-id="e8f90-130">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="e8f90-131">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="e8f90-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="e8f90-132">Contact</span><span class="sxs-lookup"><span data-stu-id="e8f90-132">Contact</span></span>](contact.md)| <span data-ttu-id="e8f90-133">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="e8f90-134">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="e8f90-134">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="e8f90-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-135">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="e8f90-136">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-136">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="e8f90-137">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="e8f90-137">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e8f90-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-138">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="e8f90-139">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-139">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="e8f90-140">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="e8f90-140">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="e8f90-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="e8f90-142">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-142">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="e8f90-143">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="e8f90-143">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="e8f90-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e8f90-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="e8f90-145">`$expand` を使用して、複数値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="e8f90-145">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="e8f90-146">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8f90-146">Properties</span></span>
| <span data-ttu-id="e8f90-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8f90-147">Property</span></span>     | <span data-ttu-id="e8f90-148">型</span><span class="sxs-lookup"><span data-stu-id="e8f90-148">Type</span></span>   |<span data-ttu-id="e8f90-149">説明</span><span class="sxs-lookup"><span data-stu-id="e8f90-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8f90-150">displayName</span><span class="sxs-lookup"><span data-stu-id="e8f90-150">displayName</span></span>|<span data-ttu-id="e8f90-151">String</span><span class="sxs-lookup"><span data-stu-id="e8f90-151">String</span></span>|<span data-ttu-id="e8f90-152">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e8f90-152">The folder's display name.</span></span>|
|<span data-ttu-id="e8f90-153">id</span><span class="sxs-lookup"><span data-stu-id="e8f90-153">id</span></span>|<span data-ttu-id="e8f90-154">文字列</span><span class="sxs-lookup"><span data-stu-id="e8f90-154">String</span></span>|<span data-ttu-id="e8f90-p101">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e8f90-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="e8f90-157">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e8f90-157">parentFolderId</span></span>|<span data-ttu-id="e8f90-158">String</span><span class="sxs-lookup"><span data-stu-id="e8f90-158">String</span></span>|<span data-ttu-id="e8f90-159">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="e8f90-159">The ID of the folder's parent folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8f90-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8f90-160">Relationships</span></span>
| <span data-ttu-id="e8f90-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8f90-161">Relationship</span></span> | <span data-ttu-id="e8f90-162">型</span><span class="sxs-lookup"><span data-stu-id="e8f90-162">Type</span></span>   |<span data-ttu-id="e8f90-163">説明</span><span class="sxs-lookup"><span data-stu-id="e8f90-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8f90-164">childFolders</span><span class="sxs-lookup"><span data-stu-id="e8f90-164">childFolders</span></span>|<span data-ttu-id="e8f90-165">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="e8f90-165">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="e8f90-p102">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e8f90-p102">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e8f90-170">contacts</span><span class="sxs-lookup"><span data-stu-id="e8f90-170">contacts</span></span>|<span data-ttu-id="e8f90-171">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="e8f90-171">[Contact](contact.md) collection</span></span>|<span data-ttu-id="e8f90-p103">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e8f90-p103">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e8f90-176">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e8f90-176">multiValueExtendedProperties</span></span>|<span data-ttu-id="e8f90-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8f90-177">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e8f90-p104">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e8f90-p104">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e8f90-181">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="e8f90-181">singleValueExtendedProperties</span></span>|<span data-ttu-id="e8f90-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8f90-182">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="e8f90-p105">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e8f90-p105">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8f90-186">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8f90-186">JSON representation</span></span>

<span data-ttu-id="e8f90-187">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e8f90-187">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="e8f90-188">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8f90-188">See also</span></span>

- [<span data-ttu-id="e8f90-189">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="e8f90-189">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="e8f90-190">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="e8f90-190">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
