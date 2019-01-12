---
title: contactFolder リソース型
description: 連絡先が格納されたフォルダーです。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 450c683d91eeb789c8c54b2bbfd38db695fbbba2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967547"
---
# <a name="contactfolder-resource-type"></a><span data-ttu-id="515dc-103">contactFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="515dc-103">contactFolder resource type</span></span>

> <span data-ttu-id="515dc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="515dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="515dc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="515dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="515dc-106">連絡先が格納されたフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="515dc-106">A folder that contains contacts.</span></span>

<span data-ttu-id="515dc-107">このリソースでは、[デルタ](../api/contactfolder-delta.md)関数を用意すれば、増分の追加、削除、更新に[デルタ クエリ](/graph/delta-query-overview)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="515dc-107">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contactfolder-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="515dc-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="515dc-108">Methods</span></span>

| <span data-ttu-id="515dc-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="515dc-109">Method</span></span>       | <span data-ttu-id="515dc-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="515dc-110">Return Type</span></span>  |<span data-ttu-id="515dc-111">説明</span><span class="sxs-lookup"><span data-stu-id="515dc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="515dc-112">contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="515dc-112">Get contactFolder</span></span>](../api/contactfolder-get.md) | [<span data-ttu-id="515dc-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-113">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="515dc-114">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="515dc-114">Get a contact folder by using the contact folder ID.</span></span>|
|[<span data-ttu-id="515dc-115">更新する</span><span class="sxs-lookup"><span data-stu-id="515dc-115">Update</span></span>](../api/contactfolder-update.md) | [<span data-ttu-id="515dc-116">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-116">contactFolder</span></span>](contactfolder.md) |<span data-ttu-id="515dc-117">contactFolder オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="515dc-117">Update contactFolder object.</span></span> |
|[<span data-ttu-id="515dc-118">削除</span><span class="sxs-lookup"><span data-stu-id="515dc-118">Delete</span></span>](../api/contactfolder-delete.md) | <span data-ttu-id="515dc-119">なし</span><span class="sxs-lookup"><span data-stu-id="515dc-119">None</span></span> |<span data-ttu-id="515dc-120">contactFolder オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="515dc-120">Delete contactFolder object.</span></span> |
|[<span data-ttu-id="515dc-121">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="515dc-121">List childFolders</span></span>](../api/contactfolder-list-childfolders.md) |<span data-ttu-id="515dc-122">[contactFolder](contactfolder.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-122">[contactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="515dc-123">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="515dc-123">Get a collection of child folders under the specified contact folder.</span></span>|
|[<span data-ttu-id="515dc-124">子 contactFolder を作成する</span><span class="sxs-lookup"><span data-stu-id="515dc-124">Create child contactFolder</span></span>](../api/contactfolder-post-childfolders.md) |[<span data-ttu-id="515dc-125">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-125">contactFolder</span></span>](contactfolder.md)| <span data-ttu-id="515dc-126">指定したフォルダーの子として新しい contactFolder を作成します。</span><span class="sxs-lookup"><span data-stu-id="515dc-126">Create a new contactFolder as a child of a specified folder.</span></span>|
|[<span data-ttu-id="515dc-127">delta</span><span class="sxs-lookup"><span data-stu-id="515dc-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="515dc-128">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="515dc-129">ユーザーのメールボックスで追加または削除された一連の連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="515dc-129">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>|
|[<span data-ttu-id="515dc-130">フォルダー内の連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="515dc-130">List contacts in folder</span></span>](../api/contactfolder-list-contacts.md) |<span data-ttu-id="515dc-131">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-131">[contact](contact.md) collection</span></span>| <span data-ttu-id="515dc-132">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得する (`.../me/contacts`) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="515dc-132">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>|
|[<span data-ttu-id="515dc-133">フォルダー内に連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="515dc-133">Create contact in folder</span></span>](../api/contactfolder-post-contacts.md) |[<span data-ttu-id="515dc-134">連絡先</span><span class="sxs-lookup"><span data-stu-id="515dc-134">contact</span></span>](contact.md)| <span data-ttu-id="515dc-135">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="515dc-135">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>|
|<span data-ttu-id="515dc-136">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="515dc-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="515dc-137">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="515dc-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="515dc-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-138">contactFolder</span></span>](contactfolder.md)  |<span data-ttu-id="515dc-139">新規または既存の contactFolder に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="515dc-139">Create one or more single-value extended properties in a new or existing contactFolder.</span></span>   |
|[<span data-ttu-id="515dc-140">単一値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="515dc-140">Get contactFolder with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="515dc-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-141">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="515dc-142">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="515dc-142">Get contactFolders that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="515dc-143">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="515dc-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="515dc-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-144">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="515dc-145">新規または既存の contactFolder に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="515dc-145">Create one or more multi-value extended properties in a new or existing contactFolder.</span></span>  |
|[<span data-ttu-id="515dc-146">複数値の拡張プロパティを持つ contactFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="515dc-146">Get contactFolder with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="515dc-147">contactFolder</span><span class="sxs-lookup"><span data-stu-id="515dc-147">contactFolder</span></span>](contactfolder.md) | <span data-ttu-id="515dc-148">`$expand` を使用して、複数値の拡張プロパティを含む contactFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="515dc-148">Get a contactFolder that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="515dc-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="515dc-149">Properties</span></span>
| <span data-ttu-id="515dc-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="515dc-150">Property</span></span>     | <span data-ttu-id="515dc-151">種類</span><span class="sxs-lookup"><span data-stu-id="515dc-151">Type</span></span>   |<span data-ttu-id="515dc-152">説明</span><span class="sxs-lookup"><span data-stu-id="515dc-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="515dc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="515dc-153">displayName</span></span>|<span data-ttu-id="515dc-154">String</span><span class="sxs-lookup"><span data-stu-id="515dc-154">String</span></span>|<span data-ttu-id="515dc-155">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="515dc-155">The folder's display name.</span></span>|
|<span data-ttu-id="515dc-156">id</span><span class="sxs-lookup"><span data-stu-id="515dc-156">id</span></span>|<span data-ttu-id="515dc-157">String</span><span class="sxs-lookup"><span data-stu-id="515dc-157">String</span></span>|<span data-ttu-id="515dc-p102">連絡先フォルダーの一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="515dc-p102">Unique identifier of the contact folder. Read-only.</span></span>|
|<span data-ttu-id="515dc-160">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="515dc-160">parentFolderId</span></span>|<span data-ttu-id="515dc-161">String</span><span class="sxs-lookup"><span data-stu-id="515dc-161">String</span></span>|<span data-ttu-id="515dc-162">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="515dc-162">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="515dc-163">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="515dc-163">wellKnownName</span></span>|<span data-ttu-id="515dc-164">string</span><span class="sxs-lookup"><span data-stu-id="515dc-164">string</span></span>|<span data-ttu-id="515dc-p103">フォルダーが認識されているフォルダーである場合、フォルダーの名前。現在、認識されている連絡先フォルダーは `contacts` のみです。</span><span class="sxs-lookup"><span data-stu-id="515dc-p103">The name of the folder if the folder is a recognized folder. Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="515dc-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="515dc-167">Relationships</span></span>
| <span data-ttu-id="515dc-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="515dc-168">Relationship</span></span> | <span data-ttu-id="515dc-169">型</span><span class="sxs-lookup"><span data-stu-id="515dc-169">Type</span></span>   |<span data-ttu-id="515dc-170">説明</span><span class="sxs-lookup"><span data-stu-id="515dc-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="515dc-171">childFolders</span><span class="sxs-lookup"><span data-stu-id="515dc-171">childFolders</span></span>|<span data-ttu-id="515dc-172">[ContactFolder](contactfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-172">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="515dc-p104">フォルダー内の子フォルダーのコレクション。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="515dc-p104">The collection of child folders in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="515dc-177">contacts</span><span class="sxs-lookup"><span data-stu-id="515dc-177">contacts</span></span>|<span data-ttu-id="515dc-178">[Contact](contact.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-178">[Contact](contact.md) collection</span></span>|<span data-ttu-id="515dc-p105">フォルダー内の連絡先。ナビゲーション プロパティ。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="515dc-p105">The contacts in the folder. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="515dc-183">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="515dc-183">multiValueExtendedProperties</span></span>|<span data-ttu-id="515dc-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-184">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="515dc-p106">contactFolder に定義された、複数値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="515dc-p106">The collection of multi-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="515dc-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="515dc-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="515dc-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="515dc-189">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="515dc-p107">contactFolder に定義された、単一値の拡張プロパティのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="515dc-p107">The collection of single-value extended properties defined for the contactFolder. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="515dc-193">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="515dc-193">JSON representation</span></span>

<span data-ttu-id="515dc-194">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="515dc-194">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="515dc-195">関連項目</span><span class="sxs-lookup"><span data-stu-id="515dc-195">See also</span></span>

- [<span data-ttu-id="515dc-196">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="515dc-196">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="515dc-197">フォルダー内のメッセージへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="515dc-197">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
