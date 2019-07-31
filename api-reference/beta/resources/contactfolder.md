---
title: contactFolder リソース型
description: 連絡先が格納されたフォルダーです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4a9fe3263bed04252e8eba5129437d0a7c155d42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973192"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="3b472-103">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="3b472-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b472-104">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="3b472-104">A folder that contains contacts.</span></span>

<span data-ttu-id="3b472-105">このリソースでは、[デルタ](../api/contactfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3b472-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="3b472-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b472-106">Methods</span></span>

| <span data-ttu-id="3b472-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b472-107">Method</span></span>       | <span data-ttu-id="3b472-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3b472-108">Return Type</span></span>  |<span data-ttu-id="3b472-109">説明</span><span class="sxs-lookup"><span data-stu-id="3b472-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b472-110">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="3b472-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="3b472-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="3b472-112">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="3b472-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="3b472-113">更新する</span><span class="sxs-lookup"><span data-stu-id="3b472-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="3b472-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="3b472-115">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b472-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="3b472-116">Delete</span><span class="sxs-lookup"><span data-stu-id="3b472-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="3b472-117">None</span><span class="sxs-lookup"><span data-stu-id="3b472-117">None</span></span> |<span data-ttu-id="3b472-118">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="3b472-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="3b472-119">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3b472-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="3b472-120">[contactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3b472-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="3b472-121">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3b472-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="3b472-122">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="3b472-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="3b472-123">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-123">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="3b472-124">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b472-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="3b472-125">delta</span><span class="sxs-lookup"><span data-stu-id="3b472-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="3b472-126">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3b472-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="3b472-127">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="3b472-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="3b472-128">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3b472-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="3b472-129">[contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3b472-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="3b472-130">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="3b472-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="3b472-131">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="3b472-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="3b472-132">contact</span><span class="sxs-lookup"><span data-stu-id="3b472-132">contact</span></span>](contact.md)| <span data-ttu-id="3b472-133">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="3b472-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="3b472-134">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="3b472-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="3b472-135">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="3b472-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="3b472-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="3b472-137">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="3b472-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="3b472-138">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="3b472-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="3b472-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="3b472-140">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b472-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="3b472-141">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="3b472-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="3b472-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="3b472-143">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="3b472-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="3b472-144">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="3b472-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="3b472-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3b472-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="3b472-146">`$expand` を使用して、複数値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b472-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b472-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b472-147">Properties</span></span>
| <span data-ttu-id="3b472-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b472-148">Property</span></span>     | <span data-ttu-id="3b472-149">型</span><span class="sxs-lookup"><span data-stu-id="3b472-149">Type</span></span>   |<span data-ttu-id="3b472-150">説明</span><span class="sxs-lookup"><span data-stu-id="3b472-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b472-151">displayName</span><span class="sxs-lookup"><span data-stu-id="3b472-151">displayName</span></span>|<span data-ttu-id="3b472-152">文字列</span><span class="sxs-lookup"><span data-stu-id="3b472-152">String</span></span>|<span data-ttu-id="3b472-153">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="3b472-153">The folder's display name.</span></span>|
|<span data-ttu-id="3b472-154">id</span><span class="sxs-lookup"><span data-stu-id="3b472-154">id</span></span>|<span data-ttu-id="3b472-155">文字列</span><span class="sxs-lookup"><span data-stu-id="3b472-155">String</span></span>|<span data-ttu-id="3b472-p101">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3b472-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="3b472-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="3b472-158">parentFolderId</span></span>|<span data-ttu-id="3b472-159">String</span><span class="sxs-lookup"><span data-stu-id="3b472-159">String</span></span>|<span data-ttu-id="3b472-160">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="3b472-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="3b472-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="3b472-161">wellKnownName</span></span>|<span data-ttu-id="3b472-162">string</span><span class="sxs-lookup"><span data-stu-id="3b472-162">string</span></span>|<span data-ttu-id="3b472-163">フォルダーが認識されているフォルダーである場合、フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="3b472-163">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="3b472-164">現在、認識されている連絡先フォルダーは `contacts` のみです。</span><span class="sxs-lookup"><span data-stu-id="3b472-164">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b472-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b472-165">Relationships</span></span>
| <span data-ttu-id="3b472-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b472-166">Relationship</span></span> | <span data-ttu-id="3b472-167">型</span><span class="sxs-lookup"><span data-stu-id="3b472-167">Type</span></span>   |<span data-ttu-id="3b472-168">説明</span><span class="sxs-lookup"><span data-stu-id="3b472-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b472-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="3b472-169">childFolders</span></span>|<span data-ttu-id="3b472-170">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="3b472-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="3b472-p103">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="3b472-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3b472-175">contacts</span><span class="sxs-lookup"><span data-stu-id="3b472-175">contacts</span></span>|<span data-ttu-id="3b472-176">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="3b472-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="3b472-p104">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="3b472-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3b472-181">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3b472-181">multiValueExtendedProperties</span></span>|<span data-ttu-id="3b472-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3b472-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3b472-p105">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="3b472-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3b472-186">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3b472-186">singleValueExtendedProperties</span></span>|<span data-ttu-id="3b472-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3b472-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3b472-p106">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="3b472-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b472-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b472-191">JSON representation</span></span>

<span data-ttu-id="3b472-192">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3b472-192">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a><span data-ttu-id="3b472-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="3b472-193">See also</span></span>

- [<span data-ttu-id="3b472-194">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="3b472-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="3b472-195">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="3b472-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
