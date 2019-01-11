---
title: person リソースの種類
description: メール、連絡先、ソーシャル ネットワークの間でのユーザーに関する情報を集計します。 ユーザーは、個人用の連絡先、ソーシャル ネットワー キングの連絡先、組織のディレクトリ、およびユーザーの最新の通信 (電子メール、Skype など) を使用できます。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: c0318986b01704501a2b7910888d6a5e962a5dca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865381"
---
# <a name="person-resource-type"></a><span data-ttu-id="7a6b1-104">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a6b1-104">person resource type</span></span>

> <span data-ttu-id="7a6b1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a6b1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a6b1-107">メール、連絡先、ソーシャル ネットワークの間でのユーザーに関する情報を集計します。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-107">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="7a6b1-108">ユーザーは、個人用の連絡先、ソーシャル ネットワー キングの連絡先、組織のディレクトリ、およびユーザーの最新の通信 (電子メール、Skype など) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-108">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="7a6b1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a6b1-109">Methods</span></span>

| <span data-ttu-id="7a6b1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="7a6b1-110">Method</span></span> | <span data-ttu-id="7a6b1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7a6b1-111">Return Type</span></span> | <span data-ttu-id="7a6b1-112">説明</span><span class="sxs-lookup"><span data-stu-id="7a6b1-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a6b1-113">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7a6b1-113">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="7a6b1-114">**人物**</span><span class="sxs-lookup"><span data-stu-id="7a6b1-114">**person**</span></span> |<span data-ttu-id="7a6b1-115">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-115">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="7a6b1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a6b1-116">Properties</span></span>

| <span data-ttu-id="7a6b1-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a6b1-117">Property</span></span> | <span data-ttu-id="7a6b1-118">種類</span><span class="sxs-lookup"><span data-stu-id="7a6b1-118">Type</span></span> | <span data-ttu-id="7a6b1-119">説明</span><span class="sxs-lookup"><span data-stu-id="7a6b1-119">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7a6b1-120">birthday</span><span class="sxs-lookup"><span data-stu-id="7a6b1-120">birthday</span></span>|<span data-ttu-id="7a6b1-121">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-121">string</span></span>|<span data-ttu-id="7a6b1-122">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-122">The person's birthday.</span></span>|
|<span data-ttu-id="7a6b1-123">companyName</span><span class="sxs-lookup"><span data-stu-id="7a6b1-123">companyName</span></span>|<span data-ttu-id="7a6b1-124">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-124">string</span></span>|<span data-ttu-id="7a6b1-125">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-125">The name of the person's company.</span></span>|
|<span data-ttu-id="7a6b1-126">department</span><span class="sxs-lookup"><span data-stu-id="7a6b1-126">department</span></span>|<span data-ttu-id="7a6b1-127">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-127">string</span></span>|<span data-ttu-id="7a6b1-128">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-128">The person's department.</span></span>|
|<span data-ttu-id="7a6b1-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7a6b1-129">displayName</span></span>|<span data-ttu-id="7a6b1-130">string</span><span class="sxs-lookup"><span data-stu-id="7a6b1-130">string</span></span>|<span data-ttu-id="7a6b1-131">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-131">The person's display name.</span></span>|
|<span data-ttu-id="7a6b1-132">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="7a6b1-132">emailAddresses</span></span>|<span data-ttu-id="7a6b1-133">[rankedEmailAddress](rankedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7a6b1-133">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="7a6b1-134">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-134">The person's email addresses.</span></span>|
|<span data-ttu-id="7a6b1-135">givenName</span><span class="sxs-lookup"><span data-stu-id="7a6b1-135">givenName</span></span>|<span data-ttu-id="7a6b1-136">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-136">string</span></span>|<span data-ttu-id="7a6b1-137">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-137">The person's given name.</span></span>|
|<span data-ttu-id="7a6b1-138">ID</span><span class="sxs-lookup"><span data-stu-id="7a6b1-138">id</span></span>|<span data-ttu-id="7a6b1-139">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-139">string</span></span>|<span data-ttu-id="7a6b1-p104">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-p104">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="7a6b1-142">isFavorite</span><span class="sxs-lookup"><span data-stu-id="7a6b1-142">isFavorite</span></span>|<span data-ttu-id="7a6b1-143">ブール</span><span class="sxs-lookup"><span data-stu-id="7a6b1-143">boolean</span></span>|<span data-ttu-id="7a6b1-144">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-144">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="7a6b1-145">mailboxType</span><span class="sxs-lookup"><span data-stu-id="7a6b1-145">mailboxType</span></span>|<span data-ttu-id="7a6b1-146">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-146">string</span></span>|<span data-ttu-id="7a6b1-147">相手の電子メール アドレスで表されるメールボックスの種類です。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-147">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="7a6b1-148">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7a6b1-148">officeLocation</span></span>|<span data-ttu-id="7a6b1-149">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-149">string</span></span>|<span data-ttu-id="7a6b1-150">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-150">The location of the person's office.</span></span>|
|<span data-ttu-id="7a6b1-151">personNotes</span><span class="sxs-lookup"><span data-stu-id="7a6b1-151">personNotes</span></span>|<span data-ttu-id="7a6b1-152">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-152">string</span></span>|<span data-ttu-id="7a6b1-153">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-153">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="7a6b1-154">personType</span><span class="sxs-lookup"><span data-stu-id="7a6b1-154">personType</span></span>|<span data-ttu-id="7a6b1-155">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-155">string</span></span>|<span data-ttu-id="7a6b1-156">配布リストなど、ユーザーの種類。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-156">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="7a6b1-157">phones</span><span class="sxs-lookup"><span data-stu-id="7a6b1-157">phones</span></span>|<span data-ttu-id="7a6b1-158">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7a6b1-158">[phone](phone.md) collection</span></span>|<span data-ttu-id="7a6b1-159">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-159">The person's phone numbers.</span></span>|
|<span data-ttu-id="7a6b1-160">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="7a6b1-160">postalAddresses</span></span>|<span data-ttu-id="7a6b1-161">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7a6b1-161">[location](location.md) collection</span></span>|<span data-ttu-id="7a6b1-162">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-162">The person's addresses.</span></span>|
|<span data-ttu-id="7a6b1-163">profession</span><span class="sxs-lookup"><span data-stu-id="7a6b1-163">profession</span></span>|<span data-ttu-id="7a6b1-164">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-164">string</span></span>|<span data-ttu-id="7a6b1-165">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-165">The person's profession.</span></span>|
|<span data-ttu-id="7a6b1-166">ソース</span><span class="sxs-lookup"><span data-stu-id="7a6b1-166">sources</span></span>|<span data-ttu-id="7a6b1-167">[personDataSource](persondatasource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7a6b1-167">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="7a6b1-168">ソース ユーザー データからのもの、たとえば、ディレクトリ、または Outlook の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-168">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="7a6b1-169">surname</span><span class="sxs-lookup"><span data-stu-id="7a6b1-169">surname</span></span>|<span data-ttu-id="7a6b1-170">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-170">string</span></span>|<span data-ttu-id="7a6b1-171">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-171">The person's surname.</span></span>|
|<span data-ttu-id="7a6b1-172">タイトル</span><span class="sxs-lookup"><span data-stu-id="7a6b1-172">title</span></span>|<span data-ttu-id="7a6b1-173">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-173">string</span></span>|<span data-ttu-id="7a6b1-174">人のタイトルです。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-174">The person's title.</span></span>|
|<span data-ttu-id="7a6b1-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a6b1-175">userPrincipalName</span></span>|<span data-ttu-id="7a6b1-176">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-176">string</span></span>|<span data-ttu-id="7a6b1-p105">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="7a6b1-181">websites</span><span class="sxs-lookup"><span data-stu-id="7a6b1-181">websites</span></span>|<span data-ttu-id="7a6b1-182">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7a6b1-182">[website](website.md) collection</span></span>|<span data-ttu-id="7a6b1-183">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-183">The person's websites.</span></span>|
|<span data-ttu-id="7a6b1-184">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="7a6b1-184">yomiCompany</span></span>|<span data-ttu-id="7a6b1-185">文字列</span><span class="sxs-lookup"><span data-stu-id="7a6b1-185">string</span></span>|<span data-ttu-id="7a6b1-186">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-186">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a6b1-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a6b1-187">Relationships</span></span>

<span data-ttu-id="7a6b1-188">なし</span><span class="sxs-lookup"><span data-stu-id="7a6b1-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a6b1-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a6b1-189">JSON representation</span></span>

<span data-ttu-id="7a6b1-190">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a6b1-190">Here is a JSON representation of the resource.</span></span>

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
