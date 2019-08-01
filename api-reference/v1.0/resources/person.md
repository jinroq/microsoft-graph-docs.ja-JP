---
title: person リソースの種類
description: メール、連絡先、ソーシャル ネットワークからの、人物に関する情報の集約です。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 66c37327f329995a84a8017625f86fde989b4e3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035547"
---
# <a name="person-resource-type"></a><span data-ttu-id="ad963-104">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad963-104">person resource type</span></span>

<span data-ttu-id="ad963-p102">メール、連絡先、ソーシャル ネットワークからの、人物に関する情報の集約です。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。</span><span class="sxs-lookup"><span data-stu-id="ad963-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="ad963-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad963-107">Methods</span></span>

| <span data-ttu-id="ad963-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ad963-108">Method</span></span> | <span data-ttu-id="ad963-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ad963-109">Return Type</span></span> | <span data-ttu-id="ad963-110">説明</span><span class="sxs-lookup"><span data-stu-id="ad963-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad963-111">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ad963-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="ad963-112">**人物**</span><span class="sxs-lookup"><span data-stu-id="ad963-112">**person**</span></span> |<span data-ttu-id="ad963-113">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="ad963-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="ad963-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad963-114">Properties</span></span>

| <span data-ttu-id="ad963-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad963-115">Property</span></span> | <span data-ttu-id="ad963-116">型</span><span class="sxs-lookup"><span data-stu-id="ad963-116">Type</span></span> | <span data-ttu-id="ad963-117">説明</span><span class="sxs-lookup"><span data-stu-id="ad963-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ad963-118">birthday</span><span class="sxs-lookup"><span data-stu-id="ad963-118">birthday</span></span>|<span data-ttu-id="ad963-119">String</span><span class="sxs-lookup"><span data-stu-id="ad963-119">String</span></span>|<span data-ttu-id="ad963-120">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="ad963-120">The person's birthday.</span></span>|
|<span data-ttu-id="ad963-121">companyName</span><span class="sxs-lookup"><span data-stu-id="ad963-121">companyName</span></span>|<span data-ttu-id="ad963-122">String</span><span class="sxs-lookup"><span data-stu-id="ad963-122">String</span></span>|<span data-ttu-id="ad963-123">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="ad963-123">The name of the person's company.</span></span>|
|<span data-ttu-id="ad963-124">department</span><span class="sxs-lookup"><span data-stu-id="ad963-124">department</span></span>|<span data-ttu-id="ad963-125">String</span><span class="sxs-lookup"><span data-stu-id="ad963-125">String</span></span>|<span data-ttu-id="ad963-126">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="ad963-126">The person's department.</span></span>|
|<span data-ttu-id="ad963-127">displayName</span><span class="sxs-lookup"><span data-stu-id="ad963-127">displayName</span></span>|<span data-ttu-id="ad963-128">String</span><span class="sxs-lookup"><span data-stu-id="ad963-128">String</span></span>|<span data-ttu-id="ad963-129">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="ad963-129">The person's display name.</span></span>|
|<span data-ttu-id="ad963-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="ad963-130">scoredEmailAddresses</span></span>|<span data-ttu-id="ad963-131">[scoredEmailAddress](scoredemailaddress.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ad963-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="ad963-132">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ad963-132">The person's email addresses.</span></span>|
|<span data-ttu-id="ad963-133">givenName</span><span class="sxs-lookup"><span data-stu-id="ad963-133">givenName</span></span>|<span data-ttu-id="ad963-134">String</span><span class="sxs-lookup"><span data-stu-id="ad963-134">String</span></span>|<span data-ttu-id="ad963-135">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="ad963-135">The person's given name.</span></span>|
|<span data-ttu-id="ad963-136">id</span><span class="sxs-lookup"><span data-stu-id="ad963-136">id</span></span>|<span data-ttu-id="ad963-137">String</span><span class="sxs-lookup"><span data-stu-id="ad963-137">String</span></span>|<span data-ttu-id="ad963-p103">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad963-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="ad963-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="ad963-140">imAddress</span></span>|<span data-ttu-id="ad963-141">String</span><span class="sxs-lookup"><span data-stu-id="ad963-141">String</span></span>|<span data-ttu-id="ad963-p104">ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad963-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="ad963-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="ad963-144">isFavorite</span></span>|<span data-ttu-id="ad963-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad963-145">Boolean</span></span>|<span data-ttu-id="ad963-146">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="ad963-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="ad963-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="ad963-147">jobTitle</span></span>|<span data-ttu-id="ad963-148">String</span><span class="sxs-lookup"><span data-stu-id="ad963-148">String</span></span>|<span data-ttu-id="ad963-149">人物の役職。</span><span class="sxs-lookup"><span data-stu-id="ad963-149">The person's job title.</span></span>|
|<span data-ttu-id="ad963-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="ad963-150">officeLocation</span></span>|<span data-ttu-id="ad963-151">String</span><span class="sxs-lookup"><span data-stu-id="ad963-151">String</span></span>|<span data-ttu-id="ad963-152">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="ad963-152">The location of the person's office.</span></span>|
|<span data-ttu-id="ad963-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="ad963-153">personNotes</span></span>|<span data-ttu-id="ad963-154">String</span><span class="sxs-lookup"><span data-stu-id="ad963-154">String</span></span>|<span data-ttu-id="ad963-155">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="ad963-155">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="ad963-156">personType</span><span class="sxs-lookup"><span data-stu-id="ad963-156">personType</span></span>|[<span data-ttu-id="ad963-157">personType</span><span class="sxs-lookup"><span data-stu-id="ad963-157">personType</span></span>](persontype.md) |<span data-ttu-id="ad963-158">人物の種類。</span><span class="sxs-lookup"><span data-stu-id="ad963-158">The type of person.</span></span>|
|<span data-ttu-id="ad963-159">phones</span><span class="sxs-lookup"><span data-stu-id="ad963-159">phones</span></span>|<span data-ttu-id="ad963-160">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ad963-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="ad963-161">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="ad963-161">The person's phone numbers.</span></span>|
|<span data-ttu-id="ad963-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="ad963-162">postalAddresses</span></span>|<span data-ttu-id="ad963-163">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ad963-163">[location](location.md) collection</span></span>|<span data-ttu-id="ad963-164">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="ad963-164">The person's addresses.</span></span>|
|<span data-ttu-id="ad963-165">profession</span><span class="sxs-lookup"><span data-stu-id="ad963-165">profession</span></span>|<span data-ttu-id="ad963-166">String</span><span class="sxs-lookup"><span data-stu-id="ad963-166">String</span></span>|<span data-ttu-id="ad963-167">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="ad963-167">The person's profession.</span></span>|
|<span data-ttu-id="ad963-168">surname</span><span class="sxs-lookup"><span data-stu-id="ad963-168">surname</span></span>|<span data-ttu-id="ad963-169">String</span><span class="sxs-lookup"><span data-stu-id="ad963-169">String</span></span>|<span data-ttu-id="ad963-170">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="ad963-170">The person's surname.</span></span>|
|<span data-ttu-id="ad963-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad963-171">userPrincipalName</span></span>|<span data-ttu-id="ad963-172">String</span><span class="sxs-lookup"><span data-stu-id="ad963-172">String</span></span>|<span data-ttu-id="ad963-p105">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="ad963-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="ad963-177">websites</span><span class="sxs-lookup"><span data-stu-id="ad963-177">websites</span></span>|<span data-ttu-id="ad963-178">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ad963-178">[website](website.md) collection</span></span>|<span data-ttu-id="ad963-179">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="ad963-179">The person's websites.</span></span>|
|<span data-ttu-id="ad963-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="ad963-180">yomiCompany</span></span>|<span data-ttu-id="ad963-181">String</span><span class="sxs-lookup"><span data-stu-id="ad963-181">String</span></span>|<span data-ttu-id="ad963-182">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="ad963-182">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad963-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad963-183">Relationships</span></span>

<span data-ttu-id="ad963-184">なし。</span><span class="sxs-lookup"><span data-stu-id="ad963-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad963-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad963-185">JSON representation</span></span>

<span data-ttu-id="ad963-186">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad963-186">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
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
