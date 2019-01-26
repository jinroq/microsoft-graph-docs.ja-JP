---
title: contactFolder リソース型
description: 連絡先が格納されたフォルダーです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a4fcb5152a3d7cb5f26214cf2b0a1e4a31dc1ffb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575871"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="41930-103">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="41930-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41930-104">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="41930-104">A folder that contains contacts.</span></span>

<span data-ttu-id="41930-105">このリソースでは、[デルタ](../api/contactfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="41930-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="41930-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="41930-106">Methods</span></span>

| <span data-ttu-id="41930-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="41930-107">Method</span></span>       | <span data-ttu-id="41930-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="41930-108">Return Type</span></span>  |<span data-ttu-id="41930-109">説明</span><span class="sxs-lookup"><span data-stu-id="41930-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41930-110">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="41930-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="41930-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="41930-112">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="41930-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="41930-113">更新する</span><span class="sxs-lookup"><span data-stu-id="41930-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="41930-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="41930-115">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="41930-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="41930-116">削除</span><span class="sxs-lookup"><span data-stu-id="41930-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="41930-117">なし</span><span class="sxs-lookup"><span data-stu-id="41930-117">None</span></span> |<span data-ttu-id="41930-118">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="41930-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="41930-119">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="41930-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="41930-120">[contactFolder](contactfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="41930-121">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="41930-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="41930-122">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="41930-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="41930-123">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-123">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="41930-124">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="41930-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="41930-125">delta</span><span class="sxs-lookup"><span data-stu-id="41930-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="41930-126">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="41930-127">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="41930-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="41930-128">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="41930-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="41930-129">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="41930-130">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="41930-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="41930-131">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="41930-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="41930-132">連絡先</span><span class="sxs-lookup"><span data-stu-id="41930-132">contact</span></span>](contact.md)| <span data-ttu-id="41930-133">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="41930-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="41930-134">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="41930-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="41930-135">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="41930-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="41930-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="41930-137">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="41930-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="41930-138">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="41930-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="41930-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="41930-140">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="41930-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="41930-141">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="41930-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="41930-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="41930-143">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="41930-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="41930-144">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="41930-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="41930-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="41930-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="41930-146">`$expand` を使用して、複数値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="41930-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="41930-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41930-147">Properties</span></span>
| <span data-ttu-id="41930-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41930-148">Property</span></span>     | <span data-ttu-id="41930-149">型</span><span class="sxs-lookup"><span data-stu-id="41930-149">Type</span></span>   |<span data-ttu-id="41930-150">説明</span><span class="sxs-lookup"><span data-stu-id="41930-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41930-151">displayName</span><span class="sxs-lookup"><span data-stu-id="41930-151">displayName</span></span>|<span data-ttu-id="41930-152">String</span><span class="sxs-lookup"><span data-stu-id="41930-152">String</span></span>|<span data-ttu-id="41930-153">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="41930-153">The folder's display name.</span></span>|
|<span data-ttu-id="41930-154">id</span><span class="sxs-lookup"><span data-stu-id="41930-154">id</span></span>|<span data-ttu-id="41930-155">String</span><span class="sxs-lookup"><span data-stu-id="41930-155">String</span></span>|<span data-ttu-id="41930-p101">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="41930-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="41930-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="41930-158">parentFolderId</span></span>|<span data-ttu-id="41930-159">String</span><span class="sxs-lookup"><span data-stu-id="41930-159">String</span></span>|<span data-ttu-id="41930-160">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="41930-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="41930-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="41930-161">wellKnownName</span></span>|<span data-ttu-id="41930-162">文字列</span><span class="sxs-lookup"><span data-stu-id="41930-162">string</span></span>|<span data-ttu-id="41930-p102">フォルダーが認識されているフォルダーである場合、フォルダーの名前。現在、認識されている連絡先フォルダーは `contacts` のみです。</span><span class="sxs-lookup"><span data-stu-id="41930-p102">The name of the folder if the folder is a recognized folder. Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41930-165">関係</span><span class="sxs-lookup"><span data-stu-id="41930-165">Relationships</span></span>
| <span data-ttu-id="41930-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41930-166">Relationship</span></span> | <span data-ttu-id="41930-167">型</span><span class="sxs-lookup"><span data-stu-id="41930-167">Type</span></span>   |<span data-ttu-id="41930-168">説明</span><span class="sxs-lookup"><span data-stu-id="41930-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41930-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="41930-169">childFolders</span></span>|<span data-ttu-id="41930-170">[ContactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="41930-p103">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41930-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="41930-175">contacts</span><span class="sxs-lookup"><span data-stu-id="41930-175">contacts</span></span>|<span data-ttu-id="41930-176">[Contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="41930-p104">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41930-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="41930-181">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="41930-181">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="41930-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="41930-p105">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41930-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="41930-186">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="41930-186">singleValueLegacyExtendedProperty</span></span>|<span data-ttu-id="41930-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="41930-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="41930-p106">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="41930-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41930-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41930-191">JSON representation</span></span>

<span data-ttu-id="41930-192">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="41930-192">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty"
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

## <a name="see-also"></a><span data-ttu-id="41930-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="41930-193">See also</span></span>

- [<span data-ttu-id="41930-194">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="41930-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="41930-195">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="41930-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
