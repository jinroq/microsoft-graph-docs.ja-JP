---
title: person リソースの種類
description: メール、連絡先、ソーシャル ネットワークの間でのユーザーに関する情報を集計します。 ユーザーは、個人用の連絡先、ソーシャル ネットワー キングの連絡先、組織のディレクトリ、およびユーザーの最新の通信 (電子メール、Skype など) を使用できます。
ms.openlocfilehash: d9533c3550ec870c887b1e447fd0daf114bcfc83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066592"
---
# <a name="person-resource-type"></a><span data-ttu-id="7fcd4-104">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7fcd4-104">person resource type</span></span>

> <span data-ttu-id="7fcd4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fcd4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fcd4-107">メール、連絡先、ソーシャル ネットワークの間でのユーザーに関する情報を集計します。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-107">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="7fcd4-108">ユーザーは、個人用の連絡先、ソーシャル ネットワー キングの連絡先、組織のディレクトリ、およびユーザーの最新の通信 (電子メール、Skype など) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-108">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="7fcd4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7fcd4-109">Methods</span></span>

| <span data-ttu-id="7fcd4-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="7fcd4-110">Method</span></span> | <span data-ttu-id="7fcd4-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7fcd4-111">Return Type</span></span> | <span data-ttu-id="7fcd4-112">説明</span><span class="sxs-lookup"><span data-stu-id="7fcd4-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7fcd4-113">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7fcd4-113">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="7fcd4-114">**人物**</span><span class="sxs-lookup"><span data-stu-id="7fcd4-114">**person**</span></span> |<span data-ttu-id="7fcd4-115">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-115">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="7fcd4-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fcd4-116">Properties</span></span>

| <span data-ttu-id="7fcd4-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fcd4-117">Property</span></span> | <span data-ttu-id="7fcd4-118">型</span><span class="sxs-lookup"><span data-stu-id="7fcd4-118">Type</span></span> | <span data-ttu-id="7fcd4-119">説明</span><span class="sxs-lookup"><span data-stu-id="7fcd4-119">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7fcd4-120">birthday</span><span class="sxs-lookup"><span data-stu-id="7fcd4-120">birthday</span></span>|<span data-ttu-id="7fcd4-121">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-121">string</span></span>|<span data-ttu-id="7fcd4-122">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-122">The person's birthday.</span></span>|
|<span data-ttu-id="7fcd4-123">companyName</span><span class="sxs-lookup"><span data-stu-id="7fcd4-123">companyName</span></span>|<span data-ttu-id="7fcd4-124">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-124">string</span></span>|<span data-ttu-id="7fcd4-125">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-125">The name of the person's company.</span></span>|
|<span data-ttu-id="7fcd4-126">department</span><span class="sxs-lookup"><span data-stu-id="7fcd4-126">department</span></span>|<span data-ttu-id="7fcd4-127">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-127">string</span></span>|<span data-ttu-id="7fcd4-128">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-128">The person's department.</span></span>|
|<span data-ttu-id="7fcd4-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7fcd4-129">displayName</span></span>|<span data-ttu-id="7fcd4-130">string</span><span class="sxs-lookup"><span data-stu-id="7fcd4-130">string</span></span>|<span data-ttu-id="7fcd4-131">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-131">The person's display name.</span></span>|
|<span data-ttu-id="7fcd4-132">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="7fcd4-132">emailAddresses</span></span>|<span data-ttu-id="7fcd4-133">[rankedEmailAddress](rankedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7fcd4-133">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="7fcd4-134">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-134">The person's email addresses.</span></span>|
|<span data-ttu-id="7fcd4-135">givenName</span><span class="sxs-lookup"><span data-stu-id="7fcd4-135">givenName</span></span>|<span data-ttu-id="7fcd4-136">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-136">string</span></span>|<span data-ttu-id="7fcd4-137">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-137">The person's given name.</span></span>|
|<span data-ttu-id="7fcd4-138">id</span><span class="sxs-lookup"><span data-stu-id="7fcd4-138">id</span></span>|<span data-ttu-id="7fcd4-139">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-139">string</span></span>|<span data-ttu-id="7fcd4-p104">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-p104">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="7fcd4-142">isFavorite</span><span class="sxs-lookup"><span data-stu-id="7fcd4-142">isFavorite</span></span>|<span data-ttu-id="7fcd4-143">ブール</span><span class="sxs-lookup"><span data-stu-id="7fcd4-143">boolean</span></span>|<span data-ttu-id="7fcd4-144">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-144">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="7fcd4-145">mailboxType</span><span class="sxs-lookup"><span data-stu-id="7fcd4-145">mailboxType</span></span>|<span data-ttu-id="7fcd4-146">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-146">string</span></span>|<span data-ttu-id="7fcd4-147">相手の電子メール アドレスで表されるメールボックスの種類です。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-147">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="7fcd4-148">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7fcd4-148">officeLocation</span></span>|<span data-ttu-id="7fcd4-149">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-149">string</span></span>|<span data-ttu-id="7fcd4-150">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-150">The location of the person's office.</span></span>|
|<span data-ttu-id="7fcd4-151">personNotes</span><span class="sxs-lookup"><span data-stu-id="7fcd4-151">personNotes</span></span>|<span data-ttu-id="7fcd4-152">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-152">string</span></span>|<span data-ttu-id="7fcd4-153">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-153">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="7fcd4-154">personType</span><span class="sxs-lookup"><span data-stu-id="7fcd4-154">personType</span></span>|<span data-ttu-id="7fcd4-155">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-155">string</span></span>|<span data-ttu-id="7fcd4-156">配布リストなど、ユーザーの種類。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-156">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="7fcd4-157">phones</span><span class="sxs-lookup"><span data-stu-id="7fcd4-157">phones</span></span>|<span data-ttu-id="7fcd4-158">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7fcd4-158">[phone](phone.md) collection</span></span>|<span data-ttu-id="7fcd4-159">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-159">The person's phone numbers.</span></span>|
|<span data-ttu-id="7fcd4-160">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="7fcd4-160">postalAddresses</span></span>|<span data-ttu-id="7fcd4-161">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7fcd4-161">[location](location.md) collection</span></span>|<span data-ttu-id="7fcd4-162">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-162">The person's addresses.</span></span>|
|<span data-ttu-id="7fcd4-163">profession</span><span class="sxs-lookup"><span data-stu-id="7fcd4-163">profession</span></span>|<span data-ttu-id="7fcd4-164">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-164">string</span></span>|<span data-ttu-id="7fcd4-165">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-165">The person's profession.</span></span>|
|<span data-ttu-id="7fcd4-166">ソース</span><span class="sxs-lookup"><span data-stu-id="7fcd4-166">sources</span></span>|<span data-ttu-id="7fcd4-167">[personDataSource](persondatasource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7fcd4-167">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="7fcd4-168">ソース ユーザー データからのもの、たとえば、ディレクトリ、または Outlook の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-168">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="7fcd4-169">surname</span><span class="sxs-lookup"><span data-stu-id="7fcd4-169">surname</span></span>|<span data-ttu-id="7fcd4-170">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-170">string</span></span>|<span data-ttu-id="7fcd4-171">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-171">The person's surname.</span></span>|
|<span data-ttu-id="7fcd4-172">タイトル</span><span class="sxs-lookup"><span data-stu-id="7fcd4-172">title</span></span>|<span data-ttu-id="7fcd4-173">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-173">string</span></span>|<span data-ttu-id="7fcd4-174">人のタイトルです。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-174">The person's title.</span></span>|
|<span data-ttu-id="7fcd4-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7fcd4-175">userPrincipalName</span></span>|<span data-ttu-id="7fcd4-176">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-176">string</span></span>|<span data-ttu-id="7fcd4-p105">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="7fcd4-181">websites</span><span class="sxs-lookup"><span data-stu-id="7fcd4-181">websites</span></span>|<span data-ttu-id="7fcd4-182">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7fcd4-182">[website](website.md) collection</span></span>|<span data-ttu-id="7fcd4-183">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-183">The person's websites.</span></span>|
|<span data-ttu-id="7fcd4-184">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="7fcd4-184">yomiCompany</span></span>|<span data-ttu-id="7fcd4-185">文字列</span><span class="sxs-lookup"><span data-stu-id="7fcd4-185">string</span></span>|<span data-ttu-id="7fcd4-186">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-186">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fcd4-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7fcd4-187">Relationships</span></span>

<span data-ttu-id="7fcd4-188">なし</span><span class="sxs-lookup"><span data-stu-id="7fcd4-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fcd4-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7fcd4-189">JSON representation</span></span>

<span data-ttu-id="7fcd4-190">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7fcd4-190">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
