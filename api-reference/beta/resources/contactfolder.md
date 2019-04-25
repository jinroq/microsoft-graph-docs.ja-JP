---
title: contactFolder リソース型
description: 連絡先が格納されたフォルダーです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 599f1765b6305d2dc4d482ec035ee4b24eb5183a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543386"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="a1000-103">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="a1000-103">contactFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1000-104">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="a1000-104">A folder that contains contacts.</span></span>

<span data-ttu-id="a1000-105">このリソースでは、[デルタ](../api/contactfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a1000-105">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="a1000-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1000-106">Methods</span></span>

| <span data-ttu-id="a1000-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1000-107">Method</span></span>       | <span data-ttu-id="a1000-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1000-108">Return Type</span></span>  |<span data-ttu-id="a1000-109">説明</span><span class="sxs-lookup"><span data-stu-id="a1000-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1000-110">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="a1000-110">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="a1000-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-111">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="a1000-112">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="a1000-112">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="a1000-113">更新する</span><span class="sxs-lookup"><span data-stu-id="a1000-113">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="a1000-114">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-114">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="a1000-115">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="a1000-115">Update contactFolder object.</span></span> |
|[<span data-ttu-id="a1000-116">削除</span><span class="sxs-lookup"><span data-stu-id="a1000-116">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="a1000-117">なし</span><span class="sxs-lookup"><span data-stu-id="a1000-117">None</span></span> |<span data-ttu-id="a1000-118">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="a1000-118">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="a1000-119">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a1000-119">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="a1000-120">[contactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1000-120">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="a1000-121">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a1000-121">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="a1000-122">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="a1000-122">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="a1000-123">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-123">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="a1000-124">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="a1000-124">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="a1000-125">delta</span><span class="sxs-lookup"><span data-stu-id="a1000-125">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="a1000-126">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1000-126">[contact](contact.md) collection</span></span>| <span data-ttu-id="a1000-127">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="a1000-127">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="a1000-128">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a1000-128">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="a1000-129">[contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1000-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="a1000-130">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="a1000-130">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="a1000-131">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="a1000-131">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="a1000-132">連絡先</span><span class="sxs-lookup"><span data-stu-id="a1000-132">contact</span></span>](contact.md)| <span data-ttu-id="a1000-133">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="a1000-133">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="a1000-134">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="a1000-134">**Extended properties**</span></span>| | |
|[<span data-ttu-id="a1000-135">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="a1000-135">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="a1000-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-136">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="a1000-137">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1000-137">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="a1000-138">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="a1000-138">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a1000-139">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-139">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="a1000-140">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="a1000-140">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="a1000-141">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="a1000-141">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="a1000-142">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-142">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="a1000-143">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1000-143">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="a1000-144">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="a1000-144">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="a1000-145">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a1000-145">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="a1000-146">`$expand` を使用して、複数値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="a1000-146">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="a1000-147">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1000-147">Properties</span></span>
| <span data-ttu-id="a1000-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1000-148">Property</span></span>     | <span data-ttu-id="a1000-149">型</span><span class="sxs-lookup"><span data-stu-id="a1000-149">Type</span></span>   |<span data-ttu-id="a1000-150">説明</span><span class="sxs-lookup"><span data-stu-id="a1000-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1000-151">displayName</span><span class="sxs-lookup"><span data-stu-id="a1000-151">displayName</span></span>|<span data-ttu-id="a1000-152">String</span><span class="sxs-lookup"><span data-stu-id="a1000-152">String</span></span>|<span data-ttu-id="a1000-153">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="a1000-153">The folder's display name.</span></span>|
|<span data-ttu-id="a1000-154">id</span><span class="sxs-lookup"><span data-stu-id="a1000-154">id</span></span>|<span data-ttu-id="a1000-155">String</span><span class="sxs-lookup"><span data-stu-id="a1000-155">String</span></span>|<span data-ttu-id="a1000-p101">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="a1000-p101">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="a1000-158">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="a1000-158">parentFolderId</span></span>|<span data-ttu-id="a1000-159">String</span><span class="sxs-lookup"><span data-stu-id="a1000-159">String</span></span>|<span data-ttu-id="a1000-160">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="a1000-160">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="a1000-161">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="a1000-161">wellKnownName</span></span>|<span data-ttu-id="a1000-162">string</span><span class="sxs-lookup"><span data-stu-id="a1000-162">string</span></span>|<span data-ttu-id="a1000-163">フォルダーが認識されているフォルダーである場合、フォルダーの名前。</span><span class="sxs-lookup"><span data-stu-id="a1000-163">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="a1000-164">現在、認識されている連絡先フォルダーは `contacts` のみです。</span><span class="sxs-lookup"><span data-stu-id="a1000-164">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1000-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1000-165">Relationships</span></span>
| <span data-ttu-id="a1000-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1000-166">Relationship</span></span> | <span data-ttu-id="a1000-167">型</span><span class="sxs-lookup"><span data-stu-id="a1000-167">Type</span></span>   |<span data-ttu-id="a1000-168">説明</span><span class="sxs-lookup"><span data-stu-id="a1000-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1000-169">childFolders</span><span class="sxs-lookup"><span data-stu-id="a1000-169">childFolders</span></span>|<span data-ttu-id="a1000-170">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="a1000-170">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="a1000-p103">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a1000-p103">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a1000-175">contacts</span><span class="sxs-lookup"><span data-stu-id="a1000-175">contacts</span></span>|<span data-ttu-id="a1000-176">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="a1000-176">[Contact](contact.md) collection</span></span>|<span data-ttu-id="a1000-p104">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a1000-p104">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a1000-181">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a1000-181">multiValueExtendedProperties</span></span>|<span data-ttu-id="a1000-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1000-182">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a1000-p105">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a1000-p105">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a1000-186">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="a1000-186">singleValueExtendedProperties</span></span>|<span data-ttu-id="a1000-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1000-187">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="a1000-p106">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="a1000-p106">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1000-191">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1000-191">JSON representation</span></span>

<span data-ttu-id="a1000-192">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a1000-192">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a1000-193">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1000-193">See also</span></span>

- [<span data-ttu-id="a1000-194">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="a1000-194">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="a1000-195">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="a1000-195">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


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
