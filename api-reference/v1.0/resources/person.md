# <a name="person-resource-type"></a><span data-ttu-id="2273e-101">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2273e-101">person resource type</span></span>

<span data-ttu-id="2273e-p101">メール、連絡先、ソーシャル ネットワークからの、人物に関する情報の集約です。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。</span><span class="sxs-lookup"><span data-stu-id="2273e-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="2273e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2273e-104">Methods</span></span>

| <span data-ttu-id="2273e-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2273e-105">Method</span></span> | <span data-ttu-id="2273e-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2273e-106">Return Type</span></span> | <span data-ttu-id="2273e-107">説明</span><span class="sxs-lookup"><span data-stu-id="2273e-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2273e-108">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2273e-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="2273e-109">**人物**</span><span class="sxs-lookup"><span data-stu-id="2273e-109">**person**</span></span> |<span data-ttu-id="2273e-110">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="2273e-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="2273e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2273e-111">Properties</span></span>

| <span data-ttu-id="2273e-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2273e-112">Property</span></span> | <span data-ttu-id="2273e-113">タイプ</span><span class="sxs-lookup"><span data-stu-id="2273e-113">Type</span></span> | <span data-ttu-id="2273e-114">説明</span><span class="sxs-lookup"><span data-stu-id="2273e-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2273e-115">birthday</span><span class="sxs-lookup"><span data-stu-id="2273e-115">birthday</span></span>|<span data-ttu-id="2273e-116">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-116">String</span></span>|<span data-ttu-id="2273e-117">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="2273e-117">The person's birthday.</span></span>|
|<span data-ttu-id="2273e-118">companyName</span><span class="sxs-lookup"><span data-stu-id="2273e-118">companyName</span></span>|<span data-ttu-id="2273e-119">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-119">String</span></span>|<span data-ttu-id="2273e-120">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="2273e-120">The name of the person's company.</span></span>|
|<span data-ttu-id="2273e-121">department</span><span class="sxs-lookup"><span data-stu-id="2273e-121">department</span></span>|<span data-ttu-id="2273e-122">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-122">String</span></span>|<span data-ttu-id="2273e-123">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="2273e-123">The person's department.</span></span>|
|<span data-ttu-id="2273e-124">displayName</span><span class="sxs-lookup"><span data-stu-id="2273e-124">displayName</span></span>|<span data-ttu-id="2273e-125">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-125">String</span></span>|<span data-ttu-id="2273e-126">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="2273e-126">The person's display name.</span></span>|
|<span data-ttu-id="2273e-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="2273e-127">scoredEmailAddresses</span></span>|<span data-ttu-id="2273e-128">[scoredEmailAddress](scoredemailaddress.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2273e-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="2273e-129">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2273e-129">The person's email addresses.</span></span>|
|<span data-ttu-id="2273e-130">givenName</span><span class="sxs-lookup"><span data-stu-id="2273e-130">givenName</span></span>|<span data-ttu-id="2273e-131">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-131">String</span></span>|<span data-ttu-id="2273e-132">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="2273e-132">The person's given name.</span></span>|
|<span data-ttu-id="2273e-133">id</span><span class="sxs-lookup"><span data-stu-id="2273e-133">id</span></span>|<span data-ttu-id="2273e-134">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-134">String</span></span>|<span data-ttu-id="2273e-p102">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2273e-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="2273e-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="2273e-137">imAddress</span></span>|<span data-ttu-id="2273e-138">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-138">String</span></span>|<span data-ttu-id="2273e-p103">ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2273e-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="2273e-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="2273e-141">isFavorite</span></span>|<span data-ttu-id="2273e-142">ブール値</span><span class="sxs-lookup"><span data-stu-id="2273e-142">Boolean</span></span>|<span data-ttu-id="2273e-143">`true` ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="2273e-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="2273e-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="2273e-144">jobTitle</span></span>|<span data-ttu-id="2273e-145">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-145">String</span></span>|<span data-ttu-id="2273e-146">人物の役職。</span><span class="sxs-lookup"><span data-stu-id="2273e-146">The person's job title.</span></span>|
|<span data-ttu-id="2273e-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2273e-147">officeLocation</span></span>|<span data-ttu-id="2273e-148">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-148">String</span></span>|<span data-ttu-id="2273e-149">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="2273e-149">The location of the person's office.</span></span>|
|<span data-ttu-id="2273e-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="2273e-150">personNotes</span></span>|<span data-ttu-id="2273e-151">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-151">String</span></span>|<span data-ttu-id="2273e-152">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="2273e-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="2273e-153">personType</span><span class="sxs-lookup"><span data-stu-id="2273e-153">personType</span></span>|[<span data-ttu-id="2273e-154">personType</span><span class="sxs-lookup"><span data-stu-id="2273e-154">personType</span></span>](persontype.md) |<span data-ttu-id="2273e-155">人物の種類。</span><span class="sxs-lookup"><span data-stu-id="2273e-155">The type of person.</span></span>|
|<span data-ttu-id="2273e-156">phones</span><span class="sxs-lookup"><span data-stu-id="2273e-156">phones</span></span>|<span data-ttu-id="2273e-157">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2273e-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="2273e-158">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="2273e-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="2273e-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="2273e-159">postalAddresses</span></span>|<span data-ttu-id="2273e-160">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2273e-160">[location](location.md) collection</span></span>|<span data-ttu-id="2273e-161">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="2273e-161">The person's addresses.</span></span>|
|<span data-ttu-id="2273e-162">profession</span><span class="sxs-lookup"><span data-stu-id="2273e-162">profession</span></span>|<span data-ttu-id="2273e-163">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-163">String</span></span>|<span data-ttu-id="2273e-164">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="2273e-164">The person's profession.</span></span>|
|<span data-ttu-id="2273e-165">surname</span><span class="sxs-lookup"><span data-stu-id="2273e-165">surname</span></span>|<span data-ttu-id="2273e-166">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-166">String</span></span>|<span data-ttu-id="2273e-167">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="2273e-167">The person's surname.</span></span>|
|<span data-ttu-id="2273e-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2273e-168">userPrincipalName</span></span>|<span data-ttu-id="2273e-169">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-169">String</span></span>|<span data-ttu-id="2273e-p104">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="2273e-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="2273e-174">websites</span><span class="sxs-lookup"><span data-stu-id="2273e-174">websites</span></span>|<span data-ttu-id="2273e-175">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2273e-175">[website](website.md) collection</span></span>|<span data-ttu-id="2273e-176">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="2273e-176">The person's websites.</span></span>|
|<span data-ttu-id="2273e-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="2273e-177">yomiCompany</span></span>|<span data-ttu-id="2273e-178">文字列</span><span class="sxs-lookup"><span data-stu-id="2273e-178">String</span></span>|<span data-ttu-id="2273e-179">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="2273e-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2273e-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2273e-180">Relationships</span></span>

<span data-ttu-id="2273e-181">なし。</span><span class="sxs-lookup"><span data-stu-id="2273e-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2273e-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2273e-182">JSON representation</span></span>

<span data-ttu-id="2273e-183">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2273e-183">The following is a JSON representation of the resource.</span></span>

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
