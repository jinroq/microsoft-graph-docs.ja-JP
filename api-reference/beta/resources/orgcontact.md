---
title: orgContact リソースの種類
description: 以下は、リソースの JSON 表記です
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071988"
---
# <a name="orgcontact-resource-type"></a><span data-ttu-id="1f6cf-103">orgContact リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f6cf-103">orgContact resource type</span></span>

> <span data-ttu-id="1f6cf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f6cf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f6cf-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f6cf-106">JSON representation</span></span>

<span data-ttu-id="1f6cf-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1f6cf-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a><span data-ttu-id="1f6cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f6cf-108">Properties</span></span>
| <span data-ttu-id="1f6cf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f6cf-109">Property</span></span>     | <span data-ttu-id="1f6cf-110">型</span><span class="sxs-lookup"><span data-stu-id="1f6cf-110">Type</span></span>   |<span data-ttu-id="1f6cf-111">説明</span><span class="sxs-lookup"><span data-stu-id="1f6cf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f6cf-112">city</span><span class="sxs-lookup"><span data-stu-id="1f6cf-112">city</span></span>|<span data-ttu-id="1f6cf-113">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-113">String</span></span>| <span data-ttu-id="1f6cf-114">連絡先が含まれている都市です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-114">The city in which the contact is located.</span></span> |
|<span data-ttu-id="1f6cf-115">country</span><span class="sxs-lookup"><span data-stu-id="1f6cf-115">country</span></span>|<span data-ttu-id="1f6cf-116">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-116">String</span></span>| <span data-ttu-id="1f6cf-117">連絡先が存在する国/地域。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-117">The country/region in which the contact is located.</span></span> |
|<span data-ttu-id="1f6cf-118">department</span><span class="sxs-lookup"><span data-stu-id="1f6cf-118">department</span></span>|<span data-ttu-id="1f6cf-119">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-119">String</span></span>| <span data-ttu-id="1f6cf-120">窓口担当者の部署の名前です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-120">The name for the department in which the contact works.</span></span> |
|<span data-ttu-id="1f6cf-121">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1f6cf-121">onPremisesSyncEnabled</span></span>|<span data-ttu-id="1f6cf-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f6cf-122">Boolean</span></span>|<span data-ttu-id="1f6cf-123">このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-123">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="1f6cf-124">displayName</span><span class="sxs-lookup"><span data-stu-id="1f6cf-124">displayName</span></span>|<span data-ttu-id="1f6cf-125">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-125">String</span></span>| <span data-ttu-id="1f6cf-126">連絡先の表示名です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-126">The display name for the contact.</span></span> |
|<span data-ttu-id="1f6cf-127">givenName</span><span class="sxs-lookup"><span data-stu-id="1f6cf-127">givenName</span></span>|<span data-ttu-id="1f6cf-128">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-128">String</span></span>| <span data-ttu-id="1f6cf-129">連絡先の指定された名前 (名)。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-129">The given name (first name) of the contact.</span></span> |
|<span data-ttu-id="1f6cf-130">jobTitle</span><span class="sxs-lookup"><span data-stu-id="1f6cf-130">jobTitle</span></span>|<span data-ttu-id="1f6cf-131">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-131">String</span></span>| <span data-ttu-id="1f6cf-132">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-132">The contact's job title.</span></span> |
|<span data-ttu-id="1f6cf-133">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1f6cf-133">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="1f6cf-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f6cf-134">DateTimeOffset</span></span>|<span data-ttu-id="1f6cf-135">最後にオブジェクトが設置ディレクトリと同期された時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-135">Indicates the last time at which the object was synced with the on-premises directory.</span></span> <span data-ttu-id="1f6cf-136">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f6cf-137">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1f6cf-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1f6cf-138">onPremisesProvisioningErrors</span><span class="sxs-lookup"><span data-stu-id="1f6cf-138">onPremisesProvisioningErrors</span></span>|<span data-ttu-id="1f6cf-139">[onPremisesProvisioningError](onpremisesprovisioningerror.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-139">[onPremisesProvisioningError](onpremisesprovisioningerror.md) collection</span></span>| <span data-ttu-id="1f6cf-140">提供処理中に同期の Microsoft 製品を使用するときのエラーです。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-140">Errors when using Microsoft synchronization product during provisioning.</span></span> |
|<span data-ttu-id="1f6cf-141">mail</span><span class="sxs-lookup"><span data-stu-id="1f6cf-141">mail</span></span>|<span data-ttu-id="1f6cf-142">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-142">String</span></span>| <span data-ttu-id="1f6cf-143">"Jeff@contoso.onmicrosoft.com"など、連絡先の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-143">The SMTP address for the contact, for example, "jeff@contoso.onmicrosoft.com".</span></span> |
|<span data-ttu-id="1f6cf-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1f6cf-144">mailNickname</span></span>|<span data-ttu-id="1f6cf-145">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-145">String</span></span>| <span data-ttu-id="1f6cf-146">連絡先の電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-146">The mail alias for the contact.</span></span> |
|<span data-ttu-id="1f6cf-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="1f6cf-147">mobilePhone</span></span>|<span data-ttu-id="1f6cf-148">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-148">String</span></span>| <span data-ttu-id="1f6cf-149">連絡先の主な携帯電話の番号です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-149">The primary cellular telephone number for the contact.</span></span> |
|<span data-ttu-id="1f6cf-150">id</span><span class="sxs-lookup"><span data-stu-id="1f6cf-150">id</span></span>|<span data-ttu-id="1f6cf-151">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-151">String</span></span>| <span data-ttu-id="1f6cf-152">連絡先の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-152">The unique identifier for the contact.</span></span> <span data-ttu-id="1f6cf-153">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-153">Read-only.</span></span>|
|<span data-ttu-id="1f6cf-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="1f6cf-154">officeLocation</span></span>|<span data-ttu-id="1f6cf-155">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-155">String</span></span>| <span data-ttu-id="1f6cf-156">ビジネスの連絡先の場所のオフィスの場所。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-156">The office location in the contact's place of business.</span></span> |
|<span data-ttu-id="1f6cf-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="1f6cf-157">postalCode</span></span>|<span data-ttu-id="1f6cf-158">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-158">String</span></span>| <span data-ttu-id="1f6cf-159">連絡先の郵送先住所の郵便番号コード。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-159">The postal code for the contact's postal address.</span></span> <span data-ttu-id="1f6cf-160">郵便番号のコードは、連絡先の国/地域に固有です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-160">The postal code is specific to the contact's country/region.</span></span> <span data-ttu-id="1f6cf-161">アメリカ合衆国では、この属性には、ZIP コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-161">In the United States of America, this attribute contains the ZIP code.</span></span> |
|<span data-ttu-id="1f6cf-162">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="1f6cf-162">proxyAddresses</span></span>|<span data-ttu-id="1f6cf-163">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-163">String collection</span></span>| <span data-ttu-id="1f6cf-164">例: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any**演算子は、複数値を持つプロパティのフィルター式に必要です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-164">For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="1f6cf-165">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-165">Read-only.</span></span> <span data-ttu-id="1f6cf-166">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-166">Not nullable.</span></span> <span data-ttu-id="1f6cf-167">$filter をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-167">Supports $filter.</span></span> |
|<span data-ttu-id="1f6cf-168">state</span><span class="sxs-lookup"><span data-stu-id="1f6cf-168">state</span></span>|<span data-ttu-id="1f6cf-169">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-169">String</span></span>| <span data-ttu-id="1f6cf-170">都道府県連絡先のアドレスにします。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-170">The state or province in the contact's address.</span></span> |
|<span data-ttu-id="1f6cf-171">streetAddress</span><span class="sxs-lookup"><span data-stu-id="1f6cf-171">streetAddress</span></span>|<span data-ttu-id="1f6cf-172">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-172">String</span></span>| <span data-ttu-id="1f6cf-173">ビジネスの連絡先の場所の住所。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-173">The street address of the contact's place of business.</span></span> |
|<span data-ttu-id="1f6cf-174">surname</span><span class="sxs-lookup"><span data-stu-id="1f6cf-174">surname</span></span>|<span data-ttu-id="1f6cf-175">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-175">String</span></span>| <span data-ttu-id="1f6cf-176">ファミリの名前 (姓) の連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-176">The contact's surname (family name or last name).</span></span> |
|<span data-ttu-id="1f6cf-177">businessPhones</span><span class="sxs-lookup"><span data-stu-id="1f6cf-177">businessPhones</span></span>|<span data-ttu-id="1f6cf-178">String</span><span class="sxs-lookup"><span data-stu-id="1f6cf-178">String</span></span>| <span data-ttu-id="1f6cf-179">ビジネスの連絡先の場所の主な電話番号。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-179">The primary telephone number of the contact's place of business.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f6cf-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f6cf-180">Relationships</span></span>
| <span data-ttu-id="1f6cf-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1f6cf-181">Relationship</span></span> | <span data-ttu-id="1f6cf-182">型</span><span class="sxs-lookup"><span data-stu-id="1f6cf-182">Type</span></span>   |<span data-ttu-id="1f6cf-183">説明</span><span class="sxs-lookup"><span data-stu-id="1f6cf-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f6cf-184">directReports</span><span class="sxs-lookup"><span data-stu-id="1f6cf-184">directReports</span></span>|<span data-ttu-id="1f6cf-185">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1f6cf-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1f6cf-186">連絡先の直属の部下。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-186">The contact's direct reports.</span></span> <span data-ttu-id="1f6cf-187">(、ユーザーおよび連絡先のマネージャー プロパティが設定された連絡先にします。) 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-187">(The users and contacts that have their manager property set to this contact.)  Read-only.</span></span> <span data-ttu-id="1f6cf-188">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-188">Nullable.</span></span>|
|<span data-ttu-id="1f6cf-189">manager</span><span class="sxs-lookup"><span data-stu-id="1f6cf-189">manager</span></span>|[<span data-ttu-id="1f6cf-190">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1f6cf-190">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1f6cf-191">ユーザーまたは連絡先は、この連絡先のマネージャーです。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-191">The user or contact that is this contact's manager.</span></span> <span data-ttu-id="1f6cf-192">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-192">Read-only.</span></span>|
|<span data-ttu-id="1f6cf-193">memberOf</span><span class="sxs-lookup"><span data-stu-id="1f6cf-193">memberOf</span></span>|<span data-ttu-id="1f6cf-194">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1f6cf-195">メンバーである連絡先のグループです。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-195">Groups that this contact is a member of.</span></span> <span data-ttu-id="1f6cf-196">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-196">Read-only.</span></span> <span data-ttu-id="1f6cf-197">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-197">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="1f6cf-198">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f6cf-198">Methods</span></span>

| <span data-ttu-id="1f6cf-199">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f6cf-199">Method</span></span>           | <span data-ttu-id="1f6cf-200">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1f6cf-200">Return Type</span></span>    |<span data-ttu-id="1f6cf-201">説明</span><span class="sxs-lookup"><span data-stu-id="1f6cf-201">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f6cf-202">OrgContact を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-202">Get orgContact</span></span>](../api/orgcontact-get.md) | [<span data-ttu-id="1f6cf-203">orgContact</span><span class="sxs-lookup"><span data-stu-id="1f6cf-203">orgContact</span></span>](orgcontact.md) |<span data-ttu-id="1f6cf-204">OrgContact オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-204">Read properties and relationships of orgContact object.</span></span>|
|[<span data-ttu-id="1f6cf-205">マネージャーを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-205">Get manager</span></span>](../api/orgcontact-get-manager.md) |[<span data-ttu-id="1f6cf-206">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1f6cf-206">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1f6cf-207">連絡先のマネージャーを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-207">Get the contact's manager.</span></span>|
|[<span data-ttu-id="1f6cf-208">List directReports</span><span class="sxs-lookup"><span data-stu-id="1f6cf-208">List directReports</span></span>](../api/orgcontact-list-directreports.md) |<span data-ttu-id="1f6cf-209">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1f6cf-209">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1f6cf-210">連絡先の直属の部下の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-210">List the contact's direct reports.</span></span>|
|[<span data-ttu-id="1f6cf-211">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1f6cf-211">List memberOf</span></span>](../api/orgcontact-list-memberof.md) |<span data-ttu-id="1f6cf-212">[directoryObject](directoryobject.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-212">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1f6cf-213">MemberOf オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-213">Get a memberOf object collection.</span></span>|
|[<span data-ttu-id="1f6cf-214">削除</span><span class="sxs-lookup"><span data-stu-id="1f6cf-214">Delete</span></span>](../api/orgcontact-delete.md) | <span data-ttu-id="1f6cf-215">なし</span><span class="sxs-lookup"><span data-stu-id="1f6cf-215">None</span></span> |<span data-ttu-id="1f6cf-216">OrgContact オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-216">Delete orgContact object.</span></span> |
|[<span data-ttu-id="1f6cf-217">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1f6cf-217">checkMemberGroups</span></span>](../api/orgcontact-checkmembergroups.md)|<span data-ttu-id="1f6cf-218">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-218">String collection</span></span>| <span data-ttu-id="1f6cf-219">グループのメンバーシップを確認します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-219">Check for group membership.</span></span> |
|[<span data-ttu-id="1f6cf-220">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1f6cf-220">getMemberGroups</span></span>](../api/orgcontact-getmembergroups.md)|<span data-ttu-id="1f6cf-221">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-221">String collection</span></span>| <span data-ttu-id="1f6cf-222">メンバーである、指定した連絡先のすべてのグループを返します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-222">Return all the groups that the specified contact is a member of.</span></span> |
|[<span data-ttu-id="1f6cf-223">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="1f6cf-223">getMemberObjects</span></span>](../api/orgcontact-getmemberobjects.md)|<span data-ttu-id="1f6cf-224">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1f6cf-224">String collection</span></span>| <span data-ttu-id="1f6cf-225">DirectoryObjects のメンバーである連絡先の一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="1f6cf-225">Returns a list of directoryObjects the contact is a member of.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->