---
title: person リソースの種類
description: メール、連絡先、ソーシャルネットワークにわたる個人に関する情報の集約。 ユーザーは、ローカルの連絡先、ソーシャルネットワーキングからの連絡先、組織のディレクトリ、および最近のコミュニケーション (電子メールや Skype など) の人物であることができます。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 32a2c9905ab52e9b229bb8673fb4a84d90a706ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561475"
---
# <a name="person-resource-type"></a><span data-ttu-id="cd564-104">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd564-104">person resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd564-105">メール、連絡先、ソーシャルネットワークにわたる個人に関する情報の集約。</span><span class="sxs-lookup"><span data-stu-id="cd564-105">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="cd564-106">ユーザーは、ローカルの連絡先、ソーシャルネットワーキングからの連絡先、組織のディレクトリ、および最近のコミュニケーション (電子メールや Skype など) の人物であることができます。</span><span class="sxs-lookup"><span data-stu-id="cd564-106">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="cd564-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd564-107">Methods</span></span>

| <span data-ttu-id="cd564-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd564-108">Method</span></span> | <span data-ttu-id="cd564-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cd564-109">Return Type</span></span> | <span data-ttu-id="cd564-110">説明</span><span class="sxs-lookup"><span data-stu-id="cd564-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd564-111">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cd564-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="cd564-112">**人物**</span><span class="sxs-lookup"><span data-stu-id="cd564-112">**person**</span></span> |<span data-ttu-id="cd564-113">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="cd564-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="cd564-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd564-114">Properties</span></span>

| <span data-ttu-id="cd564-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd564-115">Property</span></span> | <span data-ttu-id="cd564-116">型</span><span class="sxs-lookup"><span data-stu-id="cd564-116">Type</span></span> | <span data-ttu-id="cd564-117">説明</span><span class="sxs-lookup"><span data-stu-id="cd564-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cd564-118">birthday</span><span class="sxs-lookup"><span data-stu-id="cd564-118">birthday</span></span>|<span data-ttu-id="cd564-119">string</span><span class="sxs-lookup"><span data-stu-id="cd564-119">string</span></span>|<span data-ttu-id="cd564-120">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="cd564-120">The person's birthday.</span></span>|
|<span data-ttu-id="cd564-121">companyName</span><span class="sxs-lookup"><span data-stu-id="cd564-121">companyName</span></span>|<span data-ttu-id="cd564-122">string</span><span class="sxs-lookup"><span data-stu-id="cd564-122">string</span></span>|<span data-ttu-id="cd564-123">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="cd564-123">The name of the person's company.</span></span>|
|<span data-ttu-id="cd564-124">department</span><span class="sxs-lookup"><span data-stu-id="cd564-124">department</span></span>|<span data-ttu-id="cd564-125">string</span><span class="sxs-lookup"><span data-stu-id="cd564-125">string</span></span>|<span data-ttu-id="cd564-126">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="cd564-126">The person's department.</span></span>|
|<span data-ttu-id="cd564-127">displayName</span><span class="sxs-lookup"><span data-stu-id="cd564-127">displayName</span></span>|<span data-ttu-id="cd564-128">string</span><span class="sxs-lookup"><span data-stu-id="cd564-128">string</span></span>|<span data-ttu-id="cd564-129">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="cd564-129">The person's display name.</span></span>|
|<span data-ttu-id="cd564-130">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="cd564-130">emailAddresses</span></span>|<span data-ttu-id="cd564-131">[rankedemailaddress](rankedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cd564-131">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="cd564-132">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="cd564-132">The person's email addresses.</span></span>|
|<span data-ttu-id="cd564-133">givenName</span><span class="sxs-lookup"><span data-stu-id="cd564-133">givenName</span></span>|<span data-ttu-id="cd564-134">string</span><span class="sxs-lookup"><span data-stu-id="cd564-134">string</span></span>|<span data-ttu-id="cd564-135">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="cd564-135">The person's given name.</span></span>|
|<span data-ttu-id="cd564-136">id</span><span class="sxs-lookup"><span data-stu-id="cd564-136">id</span></span>|<span data-ttu-id="cd564-137">string</span><span class="sxs-lookup"><span data-stu-id="cd564-137">string</span></span>|<span data-ttu-id="cd564-138">個人の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="cd564-138">The person's unique identifier.</span></span> <span data-ttu-id="cd564-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd564-139">Read-only.</span></span>|
|<span data-ttu-id="cd564-140">isFavorite</span><span class="sxs-lookup"><span data-stu-id="cd564-140">isFavorite</span></span>|<span data-ttu-id="cd564-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="cd564-141">boolean</span></span>|<span data-ttu-id="cd564-142">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="cd564-142">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="cd564-143">mailboxType</span><span class="sxs-lookup"><span data-stu-id="cd564-143">mailboxType</span></span>|<span data-ttu-id="cd564-144">string</span><span class="sxs-lookup"><span data-stu-id="cd564-144">string</span></span>|<span data-ttu-id="cd564-145">ユーザーの電子メールアドレスによって表されるメールボックスの種類。</span><span class="sxs-lookup"><span data-stu-id="cd564-145">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="cd564-146">officeLocation</span><span class="sxs-lookup"><span data-stu-id="cd564-146">officeLocation</span></span>|<span data-ttu-id="cd564-147">string</span><span class="sxs-lookup"><span data-stu-id="cd564-147">string</span></span>|<span data-ttu-id="cd564-148">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="cd564-148">The location of the person's office.</span></span>|
|<span data-ttu-id="cd564-149">personNotes</span><span class="sxs-lookup"><span data-stu-id="cd564-149">personNotes</span></span>|<span data-ttu-id="cd564-150">string</span><span class="sxs-lookup"><span data-stu-id="cd564-150">string</span></span>|<span data-ttu-id="cd564-151">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="cd564-151">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="cd564-152">personType</span><span class="sxs-lookup"><span data-stu-id="cd564-152">personType</span></span>|<span data-ttu-id="cd564-153">string</span><span class="sxs-lookup"><span data-stu-id="cd564-153">string</span></span>|<span data-ttu-id="cd564-154">ユーザーの種類 (例: 配布リスト)。</span><span class="sxs-lookup"><span data-stu-id="cd564-154">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="cd564-155">phones</span><span class="sxs-lookup"><span data-stu-id="cd564-155">phones</span></span>|<span data-ttu-id="cd564-156">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd564-156">[phone](phone.md) collection</span></span>|<span data-ttu-id="cd564-157">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="cd564-157">The person's phone numbers.</span></span>|
|<span data-ttu-id="cd564-158">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="cd564-158">postalAddresses</span></span>|<span data-ttu-id="cd564-159">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd564-159">[location](location.md) collection</span></span>|<span data-ttu-id="cd564-160">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="cd564-160">The person's addresses.</span></span>|
|<span data-ttu-id="cd564-161">profession</span><span class="sxs-lookup"><span data-stu-id="cd564-161">profession</span></span>|<span data-ttu-id="cd564-162">string</span><span class="sxs-lookup"><span data-stu-id="cd564-162">string</span></span>|<span data-ttu-id="cd564-163">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="cd564-163">The person's profession.</span></span>|
|<span data-ttu-id="cd564-164">sources</span><span class="sxs-lookup"><span data-stu-id="cd564-164">sources</span></span>|<span data-ttu-id="cd564-165">[個人データソース](persondatasource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cd564-165">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="cd564-166">ユーザーデータの取得元となるソース (ディレクトリまたは Outlook 連絡先など)。</span><span class="sxs-lookup"><span data-stu-id="cd564-166">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="cd564-167">surname</span><span class="sxs-lookup"><span data-stu-id="cd564-167">surname</span></span>|<span data-ttu-id="cd564-168">string</span><span class="sxs-lookup"><span data-stu-id="cd564-168">string</span></span>|<span data-ttu-id="cd564-169">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="cd564-169">The person's surname.</span></span>|
|<span data-ttu-id="cd564-170">title</span><span class="sxs-lookup"><span data-stu-id="cd564-170">title</span></span>|<span data-ttu-id="cd564-171">string</span><span class="sxs-lookup"><span data-stu-id="cd564-171">string</span></span>|<span data-ttu-id="cd564-172">個人の役職。</span><span class="sxs-lookup"><span data-stu-id="cd564-172">The person's title.</span></span>|
|<span data-ttu-id="cd564-173">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cd564-173">userPrincipalName</span></span>|<span data-ttu-id="cd564-174">string</span><span class="sxs-lookup"><span data-stu-id="cd564-174">string</span></span>|<span data-ttu-id="cd564-p104">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="cd564-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="cd564-179">websites</span><span class="sxs-lookup"><span data-stu-id="cd564-179">websites</span></span>|<span data-ttu-id="cd564-180">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cd564-180">[website](website.md) collection</span></span>|<span data-ttu-id="cd564-181">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="cd564-181">The person's websites.</span></span>|
|<span data-ttu-id="cd564-182">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="cd564-182">yomiCompany</span></span>|<span data-ttu-id="cd564-183">string</span><span class="sxs-lookup"><span data-stu-id="cd564-183">string</span></span>|<span data-ttu-id="cd564-184">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="cd564-184">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd564-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cd564-185">Relationships</span></span>

<span data-ttu-id="cd564-186">なし</span><span class="sxs-lookup"><span data-stu-id="cd564-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd564-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd564-187">JSON representation</span></span>

<span data-ttu-id="cd564-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cd564-188">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
