---
title: person リソースの種類
description: メール、連絡先、ソーシャルネットワークにわたる個人に関する情報の集約。 ユーザーは、ローカルの連絡先、ソーシャルネットワーキングからの連絡先、組織のディレクトリ、および最近のコミュニケーション (電子メールや Skype など) の人物であることができます。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 762d3bf04c891c9a2388368ca90a90ce904dc6e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966162"
---
# <a name="person-resource-type"></a><span data-ttu-id="c357d-104">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c357d-104">person resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c357d-105">メール、連絡先、ソーシャルネットワークにわたる個人に関する情報の集約。</span><span class="sxs-lookup"><span data-stu-id="c357d-105">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="c357d-106">ユーザーは、ローカルの連絡先、ソーシャルネットワーキングからの連絡先、組織のディレクトリ、および最近のコミュニケーション (電子メールや Skype など) の人物であることができます。</span><span class="sxs-lookup"><span data-stu-id="c357d-106">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="c357d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c357d-107">Methods</span></span>

| <span data-ttu-id="c357d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c357d-108">Method</span></span> | <span data-ttu-id="c357d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c357d-109">Return Type</span></span> | <span data-ttu-id="c357d-110">説明</span><span class="sxs-lookup"><span data-stu-id="c357d-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="c357d-111">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c357d-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="c357d-112">**人物**</span><span class="sxs-lookup"><span data-stu-id="c357d-112">**person**</span></span> |<span data-ttu-id="c357d-113">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="c357d-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="c357d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c357d-114">Properties</span></span>

| <span data-ttu-id="c357d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c357d-115">Property</span></span> | <span data-ttu-id="c357d-116">型</span><span class="sxs-lookup"><span data-stu-id="c357d-116">Type</span></span> | <span data-ttu-id="c357d-117">説明</span><span class="sxs-lookup"><span data-stu-id="c357d-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c357d-118">birthday</span><span class="sxs-lookup"><span data-stu-id="c357d-118">birthday</span></span>|<span data-ttu-id="c357d-119">string</span><span class="sxs-lookup"><span data-stu-id="c357d-119">string</span></span>|<span data-ttu-id="c357d-120">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="c357d-120">The person's birthday.</span></span>|
|<span data-ttu-id="c357d-121">companyName</span><span class="sxs-lookup"><span data-stu-id="c357d-121">companyName</span></span>|<span data-ttu-id="c357d-122">string</span><span class="sxs-lookup"><span data-stu-id="c357d-122">string</span></span>|<span data-ttu-id="c357d-123">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="c357d-123">The name of the person's company.</span></span>|
|<span data-ttu-id="c357d-124">department</span><span class="sxs-lookup"><span data-stu-id="c357d-124">department</span></span>|<span data-ttu-id="c357d-125">string</span><span class="sxs-lookup"><span data-stu-id="c357d-125">string</span></span>|<span data-ttu-id="c357d-126">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="c357d-126">The person's department.</span></span>|
|<span data-ttu-id="c357d-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c357d-127">displayName</span></span>|<span data-ttu-id="c357d-128">string</span><span class="sxs-lookup"><span data-stu-id="c357d-128">string</span></span>|<span data-ttu-id="c357d-129">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="c357d-129">The person's display name.</span></span>|
|<span data-ttu-id="c357d-130">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="c357d-130">emailAddresses</span></span>|<span data-ttu-id="c357d-131">[Rankedemailaddress](rankedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c357d-131">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="c357d-132">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="c357d-132">The person's email addresses.</span></span>|
|<span data-ttu-id="c357d-133">givenName</span><span class="sxs-lookup"><span data-stu-id="c357d-133">givenName</span></span>|<span data-ttu-id="c357d-134">string</span><span class="sxs-lookup"><span data-stu-id="c357d-134">string</span></span>|<span data-ttu-id="c357d-135">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="c357d-135">The person's given name.</span></span>|
|<span data-ttu-id="c357d-136">id</span><span class="sxs-lookup"><span data-stu-id="c357d-136">id</span></span>|<span data-ttu-id="c357d-137">string</span><span class="sxs-lookup"><span data-stu-id="c357d-137">string</span></span>|<span data-ttu-id="c357d-p103">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c357d-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="c357d-140">isFavorite</span><span class="sxs-lookup"><span data-stu-id="c357d-140">isFavorite</span></span>|<span data-ttu-id="c357d-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="c357d-141">boolean</span></span>|<span data-ttu-id="c357d-142">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="c357d-142">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="c357d-143">mailboxType</span><span class="sxs-lookup"><span data-stu-id="c357d-143">mailboxType</span></span>|<span data-ttu-id="c357d-144">string</span><span class="sxs-lookup"><span data-stu-id="c357d-144">string</span></span>|<span data-ttu-id="c357d-145">ユーザーの電子メールアドレスによって表されるメールボックスの種類。</span><span class="sxs-lookup"><span data-stu-id="c357d-145">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="c357d-146">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c357d-146">officeLocation</span></span>|<span data-ttu-id="c357d-147">string</span><span class="sxs-lookup"><span data-stu-id="c357d-147">string</span></span>|<span data-ttu-id="c357d-148">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="c357d-148">The location of the person's office.</span></span>|
|<span data-ttu-id="c357d-149">personNotes</span><span class="sxs-lookup"><span data-stu-id="c357d-149">personNotes</span></span>|<span data-ttu-id="c357d-150">string</span><span class="sxs-lookup"><span data-stu-id="c357d-150">string</span></span>|<span data-ttu-id="c357d-151">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="c357d-151">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="c357d-152">personType</span><span class="sxs-lookup"><span data-stu-id="c357d-152">personType</span></span>|<span data-ttu-id="c357d-153">string</span><span class="sxs-lookup"><span data-stu-id="c357d-153">string</span></span>|<span data-ttu-id="c357d-154">ユーザーの種類 (例: 配布リスト)。</span><span class="sxs-lookup"><span data-stu-id="c357d-154">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="c357d-155">phones</span><span class="sxs-lookup"><span data-stu-id="c357d-155">phones</span></span>|<span data-ttu-id="c357d-156">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c357d-156">[phone](phone.md) collection</span></span>|<span data-ttu-id="c357d-157">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="c357d-157">The person's phone numbers.</span></span>|
|<span data-ttu-id="c357d-158">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="c357d-158">postalAddresses</span></span>|<span data-ttu-id="c357d-159">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c357d-159">[location](location.md) collection</span></span>|<span data-ttu-id="c357d-160">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="c357d-160">The person's addresses.</span></span>|
|<span data-ttu-id="c357d-161">profession</span><span class="sxs-lookup"><span data-stu-id="c357d-161">profession</span></span>|<span data-ttu-id="c357d-162">string</span><span class="sxs-lookup"><span data-stu-id="c357d-162">string</span></span>|<span data-ttu-id="c357d-163">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="c357d-163">The person's profession.</span></span>|
|<span data-ttu-id="c357d-164">sources</span><span class="sxs-lookup"><span data-stu-id="c357d-164">sources</span></span>|<span data-ttu-id="c357d-165">[個人データソース](persondatasource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c357d-165">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="c357d-166">ユーザーデータの取得元となるソース (ディレクトリまたは Outlook 連絡先など)。</span><span class="sxs-lookup"><span data-stu-id="c357d-166">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="c357d-167">surname</span><span class="sxs-lookup"><span data-stu-id="c357d-167">surname</span></span>|<span data-ttu-id="c357d-168">string</span><span class="sxs-lookup"><span data-stu-id="c357d-168">string</span></span>|<span data-ttu-id="c357d-169">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="c357d-169">The person's surname.</span></span>|
|<span data-ttu-id="c357d-170">title</span><span class="sxs-lookup"><span data-stu-id="c357d-170">title</span></span>|<span data-ttu-id="c357d-171">string</span><span class="sxs-lookup"><span data-stu-id="c357d-171">string</span></span>|<span data-ttu-id="c357d-172">個人の役職。</span><span class="sxs-lookup"><span data-stu-id="c357d-172">The person's title.</span></span>|
|<span data-ttu-id="c357d-173">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c357d-173">userPrincipalName</span></span>|<span data-ttu-id="c357d-174">string</span><span class="sxs-lookup"><span data-stu-id="c357d-174">string</span></span>|<span data-ttu-id="c357d-p104">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="c357d-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="c357d-179">websites</span><span class="sxs-lookup"><span data-stu-id="c357d-179">websites</span></span>|<span data-ttu-id="c357d-180">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c357d-180">[website](website.md) collection</span></span>|<span data-ttu-id="c357d-181">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="c357d-181">The person's websites.</span></span>|
|<span data-ttu-id="c357d-182">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="c357d-182">yomiCompany</span></span>|<span data-ttu-id="c357d-183">string</span><span class="sxs-lookup"><span data-stu-id="c357d-183">string</span></span>|<span data-ttu-id="c357d-184">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="c357d-184">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c357d-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c357d-185">Relationships</span></span>

<span data-ttu-id="c357d-186">なし</span><span class="sxs-lookup"><span data-stu-id="c357d-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c357d-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c357d-187">JSON representation</span></span>

<span data-ttu-id="c357d-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c357d-188">Here is a JSON representation of the resource.</span></span>

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
