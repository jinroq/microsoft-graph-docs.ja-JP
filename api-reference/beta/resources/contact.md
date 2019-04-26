---
title: contact リソース型
description: 連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 749ae9ed2e15230bd88949aff00ce07fb2cf4b8b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341197"
---
# <a name="contact-resource-type"></a><span data-ttu-id="ae21f-104">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="ae21f-104">contact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae21f-p102">連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="ae21f-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="ae21f-107">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="ae21f-107">This resource supports:</span></span>

- <span data-ttu-id="ae21f-108">[拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="ae21f-109">[変更通知](/graph/webhooks)を受信します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="ae21f-110">[デルタ](../api/contact-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae21f-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ae21f-111">JSON representation</span></span>

<span data-ttu-id="ae21f-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ae21f-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}

```
## <a name="properties"></a><span data-ttu-id="ae21f-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae21f-113">Properties</span></span>
| <span data-ttu-id="ae21f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae21f-114">Property</span></span>     | <span data-ttu-id="ae21f-115">型</span><span class="sxs-lookup"><span data-stu-id="ae21f-115">Type</span></span>   |<span data-ttu-id="ae21f-116">説明</span><span class="sxs-lookup"><span data-stu-id="ae21f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae21f-117">assistantName</span><span class="sxs-lookup"><span data-stu-id="ae21f-117">assistantName</span></span>|<span data-ttu-id="ae21f-118">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-118">String</span></span>|<span data-ttu-id="ae21f-119">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="ae21f-119">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="ae21f-120">birthday</span><span class="sxs-lookup"><span data-stu-id="ae21f-120">birthday</span></span>|<span data-ttu-id="ae21f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae21f-121">DateTimeOffset</span></span>|<span data-ttu-id="ae21f-p103">連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae21f-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ae21f-125">categories</span><span class="sxs-lookup"><span data-stu-id="ae21f-125">categories</span></span>|<span data-ttu-id="ae21f-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-126">String collection</span></span>|<span data-ttu-id="ae21f-127">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="ae21f-127">The categories associated with the contact.</span></span> <span data-ttu-id="ae21f-128">各カテゴリは、ユーザーに対して定義されている [outlookCategory](outlookcategory.md) の **displayName** プロパティに対応しています。</span><span class="sxs-lookup"><span data-stu-id="ae21f-128">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) defined for the user.</span></span>|
|<span data-ttu-id="ae21f-129">changeKey</span><span class="sxs-lookup"><span data-stu-id="ae21f-129">changeKey</span></span>|<span data-ttu-id="ae21f-130">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-130">String</span></span>|<span data-ttu-id="ae21f-p105">連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="ae21f-p105">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="ae21f-134">children</span><span class="sxs-lookup"><span data-stu-id="ae21f-134">children</span></span>|<span data-ttu-id="ae21f-135">String collection</span><span class="sxs-lookup"><span data-stu-id="ae21f-135">String collection</span></span>|<span data-ttu-id="ae21f-136">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="ae21f-136">The names of the contact's children.</span></span>|
|<span data-ttu-id="ae21f-137">companyName</span><span class="sxs-lookup"><span data-stu-id="ae21f-137">companyName</span></span>|<span data-ttu-id="ae21f-138">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-138">String</span></span>|<span data-ttu-id="ae21f-139">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="ae21f-139">The name of the contact's company.</span></span>|
|<span data-ttu-id="ae21f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae21f-140">createdDateTime</span></span>|<span data-ttu-id="ae21f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae21f-141">DateTimeOffset</span></span>|<span data-ttu-id="ae21f-p106">連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae21f-p106">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ae21f-145">department</span><span class="sxs-lookup"><span data-stu-id="ae21f-145">department</span></span>|<span data-ttu-id="ae21f-146">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-146">String</span></span>|<span data-ttu-id="ae21f-147">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="ae21f-147">The contact's department.</span></span>|
|<span data-ttu-id="ae21f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ae21f-148">displayName</span></span>|<span data-ttu-id="ae21f-149">文字列</span><span class="sxs-lookup"><span data-stu-id="ae21f-149">String</span></span>|<span data-ttu-id="ae21f-150">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="ae21f-150">The contact's display name.</span></span> <span data-ttu-id="ae21f-151">表示名は、[作成](../api/user-post-contacts.md)操作または[更新](../api/contact-update.md)操作で指定できます。</span><span class="sxs-lookup"><span data-stu-id="ae21f-151">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="ae21f-152">後で他のプロパティを更新すると、自動的に生成された値が、指定した displayName 値に上書きされる可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ae21f-152">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="ae21f-153">既存の値を保持するには、[更新](../api/contact-update.md)操作で常に displayName として含めます。</span><span class="sxs-lookup"><span data-stu-id="ae21f-153">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="ae21f-154">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="ae21f-154">emailAddresses</span></span>|<span data-ttu-id="ae21f-155">[typedEmailAddress](typedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-155">[typedEmailAddress](typedemailaddress.md) collection</span></span>|<span data-ttu-id="ae21f-156">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ae21f-156">The contact's email addresses.</span></span>|
|<span data-ttu-id="ae21f-157">fileAs</span><span class="sxs-lookup"><span data-stu-id="ae21f-157">fileAs</span></span>|<span data-ttu-id="ae21f-158">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-158">String</span></span>|<span data-ttu-id="ae21f-159">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="ae21f-159">The name the contact is filed under.</span></span>|
|<span data-ttu-id="ae21f-160">flag</span><span class="sxs-lookup"><span data-stu-id="ae21f-160">flag</span></span>|[<span data-ttu-id="ae21f-161">followUpFlag</span><span class="sxs-lookup"><span data-stu-id="ae21f-161">followupFlag</span></span>](followupflag.md)|<span data-ttu-id="ae21f-162">連絡先の状態、開始日、期限、または終了日を示すフラグ値。</span><span class="sxs-lookup"><span data-stu-id="ae21f-162">The flag value that indicates the status, start date, due date, or completion date for the contact.</span></span> |
|<span data-ttu-id="ae21f-163">gender</span><span class="sxs-lookup"><span data-stu-id="ae21f-163">gender</span></span> |<span data-ttu-id="ae21f-164">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-164">String</span></span> |<span data-ttu-id="ae21f-165">連絡先の性別。</span><span class="sxs-lookup"><span data-stu-id="ae21f-165">The contact's gender.</span></span> |
|<span data-ttu-id="ae21f-166">generation</span><span class="sxs-lookup"><span data-stu-id="ae21f-166">generation</span></span>|<span data-ttu-id="ae21f-167">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-167">String</span></span>|<span data-ttu-id="ae21f-168">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="ae21f-168">The contact's generation.</span></span>|
|<span data-ttu-id="ae21f-169">givenName</span><span class="sxs-lookup"><span data-stu-id="ae21f-169">givenName</span></span>|<span data-ttu-id="ae21f-170">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-170">String</span></span>|<span data-ttu-id="ae21f-171">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="ae21f-171">The contact's given name.</span></span>|
|<span data-ttu-id="ae21f-172">id</span><span class="sxs-lookup"><span data-stu-id="ae21f-172">id</span></span>|<span data-ttu-id="ae21f-173">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ae21f-173">String</span></span>|<span data-ttu-id="ae21f-p108">連絡先の一意識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ae21f-p108">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="ae21f-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="ae21f-176">imAddresses</span></span>|<span data-ttu-id="ae21f-177">String collection</span><span class="sxs-lookup"><span data-stu-id="ae21f-177">String collection</span></span>|<span data-ttu-id="ae21f-178">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="ae21f-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="ae21f-179">initials</span><span class="sxs-lookup"><span data-stu-id="ae21f-179">initials</span></span>|<span data-ttu-id="ae21f-180">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-180">String</span></span>|<span data-ttu-id="ae21f-181">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="ae21f-181">The contact's initials.</span></span>|
|<span data-ttu-id="ae21f-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="ae21f-182">jobTitle</span></span>|<span data-ttu-id="ae21f-183">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-183">String</span></span>|<span data-ttu-id="ae21f-184">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="ae21f-184">The contact’s job title.</span></span>|
|<span data-ttu-id="ae21f-185">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae21f-185">lastModifiedDateTime</span></span>|<span data-ttu-id="ae21f-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae21f-186">DateTimeOffset</span></span>|<span data-ttu-id="ae21f-p109">連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae21f-p109">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ae21f-190">manager</span><span class="sxs-lookup"><span data-stu-id="ae21f-190">manager</span></span>|<span data-ttu-id="ae21f-191">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-191">String</span></span>|<span data-ttu-id="ae21f-192">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="ae21f-192">The name of the contact's manager.</span></span>
|<span data-ttu-id="ae21f-193">middleName</span><span class="sxs-lookup"><span data-stu-id="ae21f-193">middleName</span></span>|<span data-ttu-id="ae21f-194">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-194">String</span></span>|<span data-ttu-id="ae21f-195">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="ae21f-195">The contact's middle name.</span></span>|
|<span data-ttu-id="ae21f-196">nickName</span><span class="sxs-lookup"><span data-stu-id="ae21f-196">nickName</span></span>|<span data-ttu-id="ae21f-197">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-197">String</span></span>|<span data-ttu-id="ae21f-198">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="ae21f-198">The contact's nickname.</span></span>|
|<span data-ttu-id="ae21f-199">officeLocation</span><span class="sxs-lookup"><span data-stu-id="ae21f-199">officeLocation</span></span>|<span data-ttu-id="ae21f-200">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-200">String</span></span>|<span data-ttu-id="ae21f-201">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="ae21f-201">The location of the contact's office.</span></span>|
|<span data-ttu-id="ae21f-202">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="ae21f-202">parentFolderId</span></span>|<span data-ttu-id="ae21f-203">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-203">String</span></span>|<span data-ttu-id="ae21f-204">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="ae21f-204">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="ae21f-205">personalNotes</span><span class="sxs-lookup"><span data-stu-id="ae21f-205">personalNotes</span></span>|<span data-ttu-id="ae21f-206">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-206">String</span></span>|<span data-ttu-id="ae21f-207">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="ae21f-207">The user's notes about the contact.</span></span>|
|<span data-ttu-id="ae21f-208">phones</span><span class="sxs-lookup"><span data-stu-id="ae21f-208">phones</span></span> |<span data-ttu-id="ae21f-209">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-209">[phone](phone.md) collection</span></span> |<span data-ttu-id="ae21f-210">自宅電話、携帯電話、勤務先電話など、連絡先に関連付けられた電話番号。</span><span class="sxs-lookup"><span data-stu-id="ae21f-210">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="ae21f-211">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="ae21f-211">postalAddresses</span></span> |<span data-ttu-id="ae21f-212">[physicalAddress](physicaladdress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-212">[physicalAddress](physicaladdress.md) collection</span></span> |<span data-ttu-id="ae21f-213">自宅住所や勤務先住所など、連絡先に関連付けられた住所。</span><span class="sxs-lookup"><span data-stu-id="ae21f-213">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="ae21f-214">profession</span><span class="sxs-lookup"><span data-stu-id="ae21f-214">profession</span></span>|<span data-ttu-id="ae21f-215">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-215">String</span></span>|<span data-ttu-id="ae21f-216">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="ae21f-216">The contact's profession.</span></span>|
|<span data-ttu-id="ae21f-217">spouseName</span><span class="sxs-lookup"><span data-stu-id="ae21f-217">spouseName</span></span>|<span data-ttu-id="ae21f-218">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-218">String</span></span>|<span data-ttu-id="ae21f-219">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="ae21f-219">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="ae21f-220">surname</span><span class="sxs-lookup"><span data-stu-id="ae21f-220">surname</span></span>|<span data-ttu-id="ae21f-221">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-221">String</span></span>|<span data-ttu-id="ae21f-222">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="ae21f-222">The contact's surname.</span></span>|
|<span data-ttu-id="ae21f-223">title</span><span class="sxs-lookup"><span data-stu-id="ae21f-223">title</span></span>|<span data-ttu-id="ae21f-224">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-224">String</span></span>|<span data-ttu-id="ae21f-225">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="ae21f-225">The contact's title.</span></span>|
|<span data-ttu-id="ae21f-226">websites</span><span class="sxs-lookup"><span data-stu-id="ae21f-226">websites</span></span> |<span data-ttu-id="ae21f-227">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-227">[website](website.md) collection</span></span>|<span data-ttu-id="ae21f-228">連絡先に関連付けられた Web サイト。</span><span class="sxs-lookup"><span data-stu-id="ae21f-228">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="ae21f-229">weddinganniversary 日</span><span class="sxs-lookup"><span data-stu-id="ae21f-229">weddingAnniversary</span></span> |<span data-ttu-id="ae21f-230">日付</span><span class="sxs-lookup"><span data-stu-id="ae21f-230">Date</span></span> |<span data-ttu-id="ae21f-231">連絡先の結婚記念日。</span><span class="sxs-lookup"><span data-stu-id="ae21f-231">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="ae21f-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="ae21f-232">yomiCompanyName</span></span>|<span data-ttu-id="ae21f-233">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-233">String</span></span>|<span data-ttu-id="ae21f-234">連絡先の会社名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="ae21f-234">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="ae21f-235">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="ae21f-235">yomiGivenName</span></span>|<span data-ttu-id="ae21f-236">String</span><span class="sxs-lookup"><span data-stu-id="ae21f-236">String</span></span>|<span data-ttu-id="ae21f-237">連絡先の名 (ファースト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="ae21f-237">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="ae21f-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="ae21f-238">yomiSurname</span></span>|<span data-ttu-id="ae21f-239">文字列</span><span class="sxs-lookup"><span data-stu-id="ae21f-239">String</span></span>|<span data-ttu-id="ae21f-240">連絡先の姓 (ラスト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="ae21f-240">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae21f-241">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae21f-241">Relationships</span></span>
| <span data-ttu-id="ae21f-242">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ae21f-242">Relationship</span></span> | <span data-ttu-id="ae21f-243">型</span><span class="sxs-lookup"><span data-stu-id="ae21f-243">Type</span></span>   |<span data-ttu-id="ae21f-244">説明</span><span class="sxs-lookup"><span data-stu-id="ae21f-244">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae21f-245">extensions</span><span class="sxs-lookup"><span data-stu-id="ae21f-245">extensions</span></span>|<span data-ttu-id="ae21f-246">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-246">[extension](extension.md) collection</span></span>|<span data-ttu-id="ae21f-247">連絡先に対して定義されているオープン拡張機能のコレクション。</span><span class="sxs-lookup"><span data-stu-id="ae21f-247">The collection of open extensions defined for the contact.</span></span> <span data-ttu-id="ae21f-248">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae21f-248">Nullable.</span></span>|
|<span data-ttu-id="ae21f-249">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ae21f-249">multiValueExtendedProperties</span></span>|<span data-ttu-id="ae21f-250">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-250">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ae21f-p111">連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae21f-p111">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ae21f-254">写真</span><span class="sxs-lookup"><span data-stu-id="ae21f-254">photo</span></span>|[<span data-ttu-id="ae21f-255">photo</span><span class="sxs-lookup"><span data-stu-id="ae21f-255">photo</span></span>](profilephoto.md)| <span data-ttu-id="ae21f-p112">連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。</span><span class="sxs-lookup"><span data-stu-id="ae21f-p112">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="ae21f-258">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="ae21f-258">singleValueExtendedProperties</span></span>|<span data-ttu-id="ae21f-259">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-259">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="ae21f-p113">連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ae21f-p113">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="ae21f-263">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae21f-263">Methods</span></span>
| <span data-ttu-id="ae21f-264">メソッド</span><span class="sxs-lookup"><span data-stu-id="ae21f-264">Method</span></span>           | <span data-ttu-id="ae21f-265">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ae21f-265">Return Type</span></span>    |<span data-ttu-id="ae21f-266">説明</span><span class="sxs-lookup"><span data-stu-id="ae21f-266">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae21f-267">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="ae21f-267">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="ae21f-268">連絡先</span><span class="sxs-lookup"><span data-stu-id="ae21f-268">contact</span></span>](contact.md) |<span data-ttu-id="ae21f-269">連絡先オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ae21f-269">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="ae21f-270">作成</span><span class="sxs-lookup"><span data-stu-id="ae21f-270">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="ae21f-271">連絡先</span><span class="sxs-lookup"><span data-stu-id="ae21f-271">contact</span></span>](contact.md) |<span data-ttu-id="ae21f-272">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-272">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="ae21f-273">更新する</span><span class="sxs-lookup"><span data-stu-id="ae21f-273">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="ae21f-274">連絡先</span><span class="sxs-lookup"><span data-stu-id="ae21f-274">contact</span></span>](contact.md) |<span data-ttu-id="ae21f-275">連絡先オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-275">Update contact object.</span></span> |
|[<span data-ttu-id="ae21f-276">削除</span><span class="sxs-lookup"><span data-stu-id="ae21f-276">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="ae21f-277">なし</span><span class="sxs-lookup"><span data-stu-id="ae21f-277">None</span></span> |<span data-ttu-id="ae21f-278">連絡先オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-278">Delete contact object.</span></span> |
|[<span data-ttu-id="ae21f-279">delta</span><span class="sxs-lookup"><span data-stu-id="ae21f-279">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="ae21f-280">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-280">[contact](contact.md) collection</span></span>| <span data-ttu-id="ae21f-281">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-281">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="ae21f-282">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="ae21f-282">**Open extensions**</span></span>| | |
|[<span data-ttu-id="ae21f-283">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="ae21f-283">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="ae21f-284">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="ae21f-284">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="ae21f-285">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-285">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="ae21f-286">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="ae21f-286">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="ae21f-287">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae21f-287">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="ae21f-288">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-288">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="ae21f-289">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="ae21f-289">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="ae21f-290">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="ae21f-290">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="ae21f-291">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-291">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="ae21f-292">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="ae21f-292">**Extended properties**</span></span>| | |
|[<span data-ttu-id="ae21f-293">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="ae21f-293">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="ae21f-294">連絡先</span><span class="sxs-lookup"><span data-stu-id="ae21f-294">contact</span></span>](contact.md)  |<span data-ttu-id="ae21f-295">新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-295">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="ae21f-296">単一値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="ae21f-296">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ae21f-297">contact</span><span class="sxs-lookup"><span data-stu-id="ae21f-297">contact</span></span>](contact.md) | <span data-ttu-id="ae21f-298">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-298">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="ae21f-299">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="ae21f-299">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="ae21f-300">連絡先</span><span class="sxs-lookup"><span data-stu-id="ae21f-300">contact</span></span>](contact.md) | <span data-ttu-id="ae21f-301">新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-301">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="ae21f-302">複数値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="ae21f-302">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="ae21f-303">contact</span><span class="sxs-lookup"><span data-stu-id="ae21f-303">contact</span></span>](contact.md) | <span data-ttu-id="ae21f-304">`$expand` を使用して、複数値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="ae21f-304">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="ae21f-305">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae21f-305">See also</span></span>

- [<span data-ttu-id="ae21f-306">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="ae21f-306">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="ae21f-307">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="ae21f-307">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="ae21f-308">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="ae21f-308">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ae21f-309">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="ae21f-309">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ae21f-310">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="ae21f-310">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
