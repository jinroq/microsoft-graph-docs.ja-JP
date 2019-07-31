---
title: contact リソース型
description: 連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8eb692a3671672b82891a66531c64df1fcaa0e5c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012885"
---
# <a name="contact-resource-type"></a><span data-ttu-id="9a85e-104">contact リソース型</span><span class="sxs-lookup"><span data-stu-id="9a85e-104">contact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a85e-p102">連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="9a85e-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="9a85e-107">このリソースは以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="9a85e-107">This resource supports:</span></span>

- <span data-ttu-id="9a85e-108">[拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="9a85e-109">[変更通知](/graph/webhooks)を受信します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="9a85e-110">[デルタ](../api/contact-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a85e-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a85e-111">JSON representation</span></span>

<span data-ttu-id="9a85e-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9a85e-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9a85e-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a85e-113">Properties</span></span>
| <span data-ttu-id="9a85e-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a85e-114">Property</span></span>     | <span data-ttu-id="9a85e-115">型</span><span class="sxs-lookup"><span data-stu-id="9a85e-115">Type</span></span>   |<span data-ttu-id="9a85e-116">説明</span><span class="sxs-lookup"><span data-stu-id="9a85e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a85e-117">assistantName</span><span class="sxs-lookup"><span data-stu-id="9a85e-117">assistantName</span></span>|<span data-ttu-id="9a85e-118">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-118">String</span></span>|<span data-ttu-id="9a85e-119">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="9a85e-119">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="9a85e-120">birthday</span><span class="sxs-lookup"><span data-stu-id="9a85e-120">birthday</span></span>|<span data-ttu-id="9a85e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a85e-121">DateTimeOffset</span></span>|<span data-ttu-id="9a85e-p103">連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a85e-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a85e-125">categories</span><span class="sxs-lookup"><span data-stu-id="9a85e-125">categories</span></span>|<span data-ttu-id="9a85e-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-126">String collection</span></span>|<span data-ttu-id="9a85e-127">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="9a85e-127">The categories associated with the contact.</span></span> <span data-ttu-id="9a85e-128">各カテゴリは、ユーザーに対して定義されている [outlookCategory](outlookcategory.md) の **displayName** プロパティに対応しています。</span><span class="sxs-lookup"><span data-stu-id="9a85e-128">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) defined for the user.</span></span>|
|<span data-ttu-id="9a85e-129">changeKey</span><span class="sxs-lookup"><span data-stu-id="9a85e-129">changeKey</span></span>|<span data-ttu-id="9a85e-130">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-130">String</span></span>|<span data-ttu-id="9a85e-p105">連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="9a85e-p105">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="9a85e-134">children</span><span class="sxs-lookup"><span data-stu-id="9a85e-134">children</span></span>|<span data-ttu-id="9a85e-135">String collection</span><span class="sxs-lookup"><span data-stu-id="9a85e-135">String collection</span></span>|<span data-ttu-id="9a85e-136">連絡先の子供の名前。</span><span class="sxs-lookup"><span data-stu-id="9a85e-136">The names of the contact's children.</span></span>|
|<span data-ttu-id="9a85e-137">companyName</span><span class="sxs-lookup"><span data-stu-id="9a85e-137">companyName</span></span>|<span data-ttu-id="9a85e-138">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-138">String</span></span>|<span data-ttu-id="9a85e-139">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="9a85e-139">The name of the contact's company.</span></span>|
|<span data-ttu-id="9a85e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a85e-140">createdDateTime</span></span>|<span data-ttu-id="9a85e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a85e-141">DateTimeOffset</span></span>|<span data-ttu-id="9a85e-p106">連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a85e-p106">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a85e-145">department</span><span class="sxs-lookup"><span data-stu-id="9a85e-145">department</span></span>|<span data-ttu-id="9a85e-146">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-146">String</span></span>|<span data-ttu-id="9a85e-147">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="9a85e-147">The contact's department.</span></span>|
|<span data-ttu-id="9a85e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="9a85e-148">displayName</span></span>|<span data-ttu-id="9a85e-149">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9a85e-149">String</span></span>|<span data-ttu-id="9a85e-150">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="9a85e-150">The contact's display name.</span></span> <span data-ttu-id="9a85e-151">[[作成]](../api/user-post-contacts.md) または [[更新]](../api/contact-update.md) の操作で表示名を指定できます。</span><span class="sxs-lookup"><span data-stu-id="9a85e-151">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="9a85e-152">後で他のプロパティを更新すると、指定した displayName 値が自動的に生成された値に上書きされますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="9a85e-152">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="9a85e-153">既存の値を保持するには、[[更新]](../api/contact-update.md) 操作で必ずその値を displayName として含めてください。</span><span class="sxs-lookup"><span data-stu-id="9a85e-153">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="9a85e-154">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="9a85e-154">emailAddresses</span></span>|<span data-ttu-id="9a85e-155">[typedEmailAddress](typedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-155">[typedEmailAddress](typedemailaddress.md) collection</span></span>|<span data-ttu-id="9a85e-156">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="9a85e-156">The contact's email addresses.</span></span>|
|<span data-ttu-id="9a85e-157">fileAs</span><span class="sxs-lookup"><span data-stu-id="9a85e-157">fileAs</span></span>|<span data-ttu-id="9a85e-158">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-158">String</span></span>|<span data-ttu-id="9a85e-159">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="9a85e-159">The name the contact is filed under.</span></span>|
|<span data-ttu-id="9a85e-160">flag</span><span class="sxs-lookup"><span data-stu-id="9a85e-160">flag</span></span>|[<span data-ttu-id="9a85e-161">followUpFlag</span><span class="sxs-lookup"><span data-stu-id="9a85e-161">followupFlag</span></span>](followupflag.md)|<span data-ttu-id="9a85e-162">連絡先の状態、開始日、期限、または終了日を示すフラグ値。</span><span class="sxs-lookup"><span data-stu-id="9a85e-162">The flag value that indicates the status, start date, due date, or completion date for the contact.</span></span> |
|<span data-ttu-id="9a85e-163">gender</span><span class="sxs-lookup"><span data-stu-id="9a85e-163">gender</span></span> |<span data-ttu-id="9a85e-164">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-164">String</span></span> |<span data-ttu-id="9a85e-165">連絡先の性別。</span><span class="sxs-lookup"><span data-stu-id="9a85e-165">The contact's gender.</span></span> |
|<span data-ttu-id="9a85e-166">generation</span><span class="sxs-lookup"><span data-stu-id="9a85e-166">generation</span></span>|<span data-ttu-id="9a85e-167">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-167">String</span></span>|<span data-ttu-id="9a85e-168">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="9a85e-168">The contact's generation.</span></span>|
|<span data-ttu-id="9a85e-169">givenName</span><span class="sxs-lookup"><span data-stu-id="9a85e-169">givenName</span></span>|<span data-ttu-id="9a85e-170">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-170">String</span></span>|<span data-ttu-id="9a85e-171">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="9a85e-171">The contact's given name.</span></span>|
|<span data-ttu-id="9a85e-172">id</span><span class="sxs-lookup"><span data-stu-id="9a85e-172">id</span></span>|<span data-ttu-id="9a85e-173">文字列</span><span class="sxs-lookup"><span data-stu-id="9a85e-173">String</span></span>| <span data-ttu-id="9a85e-174">連絡先の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="9a85e-174">Unique identifier for the contact.</span></span> <span data-ttu-id="9a85e-175">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)]読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9a85e-175">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Read-only.</span></span> |
|<span data-ttu-id="9a85e-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="9a85e-176">imAddresses</span></span>|<span data-ttu-id="9a85e-177">String collection</span><span class="sxs-lookup"><span data-stu-id="9a85e-177">String collection</span></span>|<span data-ttu-id="9a85e-178">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="9a85e-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="9a85e-179">initials</span><span class="sxs-lookup"><span data-stu-id="9a85e-179">initials</span></span>|<span data-ttu-id="9a85e-180">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-180">String</span></span>|<span data-ttu-id="9a85e-181">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="9a85e-181">The contact's initials.</span></span>|
|<span data-ttu-id="9a85e-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="9a85e-182">jobTitle</span></span>|<span data-ttu-id="9a85e-183">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-183">String</span></span>|<span data-ttu-id="9a85e-184">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="9a85e-184">The contact’s job title.</span></span>|
|<span data-ttu-id="9a85e-185">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a85e-185">lastModifiedDateTime</span></span>|<span data-ttu-id="9a85e-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a85e-186">DateTimeOffset</span></span>|<span data-ttu-id="9a85e-p109">連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a85e-p109">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a85e-190">manager</span><span class="sxs-lookup"><span data-stu-id="9a85e-190">manager</span></span>|<span data-ttu-id="9a85e-191">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-191">String</span></span>|<span data-ttu-id="9a85e-192">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="9a85e-192">The name of the contact's manager.</span></span>
|<span data-ttu-id="9a85e-193">middleName</span><span class="sxs-lookup"><span data-stu-id="9a85e-193">middleName</span></span>|<span data-ttu-id="9a85e-194">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-194">String</span></span>|<span data-ttu-id="9a85e-195">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="9a85e-195">The contact's middle name.</span></span>|
|<span data-ttu-id="9a85e-196">nickName</span><span class="sxs-lookup"><span data-stu-id="9a85e-196">nickName</span></span>|<span data-ttu-id="9a85e-197">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-197">String</span></span>|<span data-ttu-id="9a85e-198">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="9a85e-198">The contact's nickname.</span></span>|
|<span data-ttu-id="9a85e-199">officeLocation</span><span class="sxs-lookup"><span data-stu-id="9a85e-199">officeLocation</span></span>|<span data-ttu-id="9a85e-200">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-200">String</span></span>|<span data-ttu-id="9a85e-201">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="9a85e-201">The location of the contact's office.</span></span>|
|<span data-ttu-id="9a85e-202">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="9a85e-202">parentFolderId</span></span>|<span data-ttu-id="9a85e-203">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-203">String</span></span>|<span data-ttu-id="9a85e-204">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="9a85e-204">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="9a85e-205">personalNotes</span><span class="sxs-lookup"><span data-stu-id="9a85e-205">personalNotes</span></span>|<span data-ttu-id="9a85e-206">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-206">String</span></span>|<span data-ttu-id="9a85e-207">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="9a85e-207">The user's notes about the contact.</span></span>|
|<span data-ttu-id="9a85e-208">phones</span><span class="sxs-lookup"><span data-stu-id="9a85e-208">phones</span></span> |<span data-ttu-id="9a85e-209">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-209">[phone](phone.md) collection</span></span> |<span data-ttu-id="9a85e-210">自宅電話、携帯電話、勤務先電話など、連絡先に関連付けられた電話番号。</span><span class="sxs-lookup"><span data-stu-id="9a85e-210">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="9a85e-211">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="9a85e-211">postalAddresses</span></span> |<span data-ttu-id="9a85e-212">[physicalAddress](physicaladdress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-212">[physicalAddress](physicaladdress.md) collection</span></span> |<span data-ttu-id="9a85e-213">自宅住所や勤務先住所など、連絡先に関連付けられた住所。</span><span class="sxs-lookup"><span data-stu-id="9a85e-213">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="9a85e-214">profession</span><span class="sxs-lookup"><span data-stu-id="9a85e-214">profession</span></span>|<span data-ttu-id="9a85e-215">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-215">String</span></span>|<span data-ttu-id="9a85e-216">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="9a85e-216">The contact's profession.</span></span>|
|<span data-ttu-id="9a85e-217">spouseName</span><span class="sxs-lookup"><span data-stu-id="9a85e-217">spouseName</span></span>|<span data-ttu-id="9a85e-218">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-218">String</span></span>|<span data-ttu-id="9a85e-219">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="9a85e-219">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="9a85e-220">姓</span><span class="sxs-lookup"><span data-stu-id="9a85e-220">surname</span></span>|<span data-ttu-id="9a85e-221">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-221">String</span></span>|<span data-ttu-id="9a85e-222">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="9a85e-222">The contact's surname.</span></span>|
|<span data-ttu-id="9a85e-223">title</span><span class="sxs-lookup"><span data-stu-id="9a85e-223">title</span></span>|<span data-ttu-id="9a85e-224">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-224">String</span></span>|<span data-ttu-id="9a85e-225">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="9a85e-225">The contact's title.</span></span>|
|<span data-ttu-id="9a85e-226">websites</span><span class="sxs-lookup"><span data-stu-id="9a85e-226">websites</span></span> |<span data-ttu-id="9a85e-227">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-227">[website](website.md) collection</span></span>|<span data-ttu-id="9a85e-228">連絡先に関連付けられた Web サイト。</span><span class="sxs-lookup"><span data-stu-id="9a85e-228">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="9a85e-229">weddingAnniversary 日</span><span class="sxs-lookup"><span data-stu-id="9a85e-229">weddingAnniversary</span></span> |<span data-ttu-id="9a85e-230">日付</span><span class="sxs-lookup"><span data-stu-id="9a85e-230">Date</span></span> |<span data-ttu-id="9a85e-231">連絡先の結婚記念日。</span><span class="sxs-lookup"><span data-stu-id="9a85e-231">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="9a85e-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="9a85e-232">yomiCompanyName</span></span>|<span data-ttu-id="9a85e-233">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-233">String</span></span>|<span data-ttu-id="9a85e-234">連絡先の会社名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="9a85e-234">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="9a85e-235">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="9a85e-235">yomiGivenName</span></span>|<span data-ttu-id="9a85e-236">文字列</span><span class="sxs-lookup"><span data-stu-id="9a85e-236">String</span></span>|<span data-ttu-id="9a85e-237">連絡先の名 (ファースト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="9a85e-237">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="9a85e-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="9a85e-238">yomiSurname</span></span>|<span data-ttu-id="9a85e-239">String</span><span class="sxs-lookup"><span data-stu-id="9a85e-239">String</span></span>|<span data-ttu-id="9a85e-240">連絡先の姓 (ラスト ネーム) の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="9a85e-240">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a85e-241">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9a85e-241">Relationships</span></span>
| <span data-ttu-id="9a85e-242">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9a85e-242">Relationship</span></span> | <span data-ttu-id="9a85e-243">型</span><span class="sxs-lookup"><span data-stu-id="9a85e-243">Type</span></span>   |<span data-ttu-id="9a85e-244">説明</span><span class="sxs-lookup"><span data-stu-id="9a85e-244">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a85e-245">extensions</span><span class="sxs-lookup"><span data-stu-id="9a85e-245">extensions</span></span>|<span data-ttu-id="9a85e-246">[extension](extension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-246">[extension](extension.md) collection</span></span>|<span data-ttu-id="9a85e-247">連絡先に対して定義されているオープン拡張機能のコレクション。</span><span class="sxs-lookup"><span data-stu-id="9a85e-247">The collection of open extensions defined for the contact.</span></span> <span data-ttu-id="9a85e-248">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9a85e-248">Nullable.</span></span>|
|<span data-ttu-id="9a85e-249">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9a85e-249">multiValueExtendedProperties</span></span>|<span data-ttu-id="9a85e-250">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="9a85e-250">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="9a85e-p111">連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9a85e-p111">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9a85e-254">写真</span><span class="sxs-lookup"><span data-stu-id="9a85e-254">photo</span></span>|[<span data-ttu-id="9a85e-255">photo</span><span class="sxs-lookup"><span data-stu-id="9a85e-255">photo</span></span>](profilephoto.md)| <span data-ttu-id="9a85e-p112">連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。</span><span class="sxs-lookup"><span data-stu-id="9a85e-p112">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="9a85e-258">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="9a85e-258">singleValueExtendedProperties</span></span>|<span data-ttu-id="9a85e-259">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="9a85e-259">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="9a85e-p113">連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="9a85e-p113">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="9a85e-263">メソッド</span><span class="sxs-lookup"><span data-stu-id="9a85e-263">Methods</span></span>
| <span data-ttu-id="9a85e-264">メソッド</span><span class="sxs-lookup"><span data-stu-id="9a85e-264">Method</span></span>           | <span data-ttu-id="9a85e-265">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9a85e-265">Return Type</span></span>    |<span data-ttu-id="9a85e-266">説明</span><span class="sxs-lookup"><span data-stu-id="9a85e-266">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a85e-267">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9a85e-267">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="9a85e-268">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-268">contact</span></span>](contact.md) |<span data-ttu-id="9a85e-269">連絡先オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9a85e-269">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="9a85e-270">作成</span><span class="sxs-lookup"><span data-stu-id="9a85e-270">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="9a85e-271">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-271">contact</span></span>](contact.md) |<span data-ttu-id="9a85e-272">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-272">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="9a85e-273">更新する</span><span class="sxs-lookup"><span data-stu-id="9a85e-273">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="9a85e-274">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-274">contact</span></span>](contact.md) |<span data-ttu-id="9a85e-275">連絡先オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-275">Update contact object.</span></span> |
|[<span data-ttu-id="9a85e-276">削除</span><span class="sxs-lookup"><span data-stu-id="9a85e-276">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="9a85e-277">なし</span><span class="sxs-lookup"><span data-stu-id="9a85e-277">None</span></span> |<span data-ttu-id="9a85e-278">連絡先オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-278">Delete contact object.</span></span> |
|[<span data-ttu-id="9a85e-279">delta</span><span class="sxs-lookup"><span data-stu-id="9a85e-279">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="9a85e-280">[contact](contact.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-280">[contact](contact.md) collection</span></span>| <span data-ttu-id="9a85e-281">指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-281">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="9a85e-282">**オープン拡張機能**</span><span class="sxs-lookup"><span data-stu-id="9a85e-282">**Open extensions**</span></span>| | |
|[<span data-ttu-id="9a85e-283">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="9a85e-283">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="9a85e-284">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="9a85e-284">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="9a85e-285">オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-285">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="9a85e-286">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="9a85e-286">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="9a85e-287">[openTypeExtension](opentypeextension.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a85e-287">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="9a85e-288">拡張機能の名前で識別されるオープン拡張機能を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-288">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="9a85e-289">**スキーマ拡張機能**</span><span class="sxs-lookup"><span data-stu-id="9a85e-289">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="9a85e-290">スキーマ拡張機能の値を追加する</span><span class="sxs-lookup"><span data-stu-id="9a85e-290">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="9a85e-291">スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-291">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="9a85e-292">**拡張プロパティ**</span><span class="sxs-lookup"><span data-stu-id="9a85e-292">**Extended properties**</span></span>| | |
|[<span data-ttu-id="9a85e-293">単一値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="9a85e-293">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="9a85e-294">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-294">contact</span></span>](contact.md)  |<span data-ttu-id="9a85e-295">新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-295">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="9a85e-296">単一値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9a85e-296">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9a85e-297">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-297">contact</span></span>](contact.md) | <span data-ttu-id="9a85e-298">`$expand` または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-298">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="9a85e-299">複数値の拡張プロパティを作成する</span><span class="sxs-lookup"><span data-stu-id="9a85e-299">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="9a85e-300">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-300">contact</span></span>](contact.md) | <span data-ttu-id="9a85e-301">新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-301">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="9a85e-302">複数値の拡張プロパティを持つ連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9a85e-302">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9a85e-303">contact</span><span class="sxs-lookup"><span data-stu-id="9a85e-303">contact</span></span>](contact.md) | <span data-ttu-id="9a85e-304">`$expand` を使用して、複数値の拡張プロパティを含む連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="9a85e-304">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="9a85e-305">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a85e-305">See also</span></span>

- [<span data-ttu-id="9a85e-306">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="9a85e-306">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="9a85e-307">フォルダー内のメッセージへの増分変更を取得する</span><span class="sxs-lookup"><span data-stu-id="9a85e-307">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="9a85e-308">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="9a85e-308">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9a85e-309">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="9a85e-309">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9a85e-310">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="9a85e-310">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
