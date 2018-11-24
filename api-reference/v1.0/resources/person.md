# <a name="person-resource-type"></a><span data-ttu-id="be779-101">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be779-101">person resource type</span></span>

<span data-ttu-id="be779-p101">メール、連絡先、ソーシャル ネットワークからの、人物に関する情報の集約です。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。</span><span class="sxs-lookup"><span data-stu-id="be779-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="be779-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="be779-104">Methods</span></span>

| <span data-ttu-id="be779-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="be779-105">Method</span></span> | <span data-ttu-id="be779-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="be779-106">Return Type</span></span> | <span data-ttu-id="be779-107">説明</span><span class="sxs-lookup"><span data-stu-id="be779-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="be779-108">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="be779-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="be779-109">**人物**</span><span class="sxs-lookup"><span data-stu-id="be779-109">**person**</span></span> |<span data-ttu-id="be779-110">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="be779-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="be779-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be779-111">Properties</span></span>

| <span data-ttu-id="be779-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be779-112">Property</span></span> | <span data-ttu-id="be779-113">型</span><span class="sxs-lookup"><span data-stu-id="be779-113">Type</span></span> | <span data-ttu-id="be779-114">説明</span><span class="sxs-lookup"><span data-stu-id="be779-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="be779-115">birthday</span><span class="sxs-lookup"><span data-stu-id="be779-115">birthday</span></span>|<span data-ttu-id="be779-116">String</span><span class="sxs-lookup"><span data-stu-id="be779-116">String</span></span>|<span data-ttu-id="be779-117">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="be779-117">The person's birthday.</span></span>|
|<span data-ttu-id="be779-118">companyName</span><span class="sxs-lookup"><span data-stu-id="be779-118">companyName</span></span>|<span data-ttu-id="be779-119">String</span><span class="sxs-lookup"><span data-stu-id="be779-119">String</span></span>|<span data-ttu-id="be779-120">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="be779-120">The name of the person's company.</span></span>|
|<span data-ttu-id="be779-121">department</span><span class="sxs-lookup"><span data-stu-id="be779-121">department</span></span>|<span data-ttu-id="be779-122">String</span><span class="sxs-lookup"><span data-stu-id="be779-122">String</span></span>|<span data-ttu-id="be779-123">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="be779-123">The person's department.</span></span>|
|<span data-ttu-id="be779-124">displayName</span><span class="sxs-lookup"><span data-stu-id="be779-124">displayName</span></span>|<span data-ttu-id="be779-125">String</span><span class="sxs-lookup"><span data-stu-id="be779-125">String</span></span>|<span data-ttu-id="be779-126">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="be779-126">The person's display name.</span></span>|
|<span data-ttu-id="be779-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="be779-127">scoredEmailAddresses</span></span>|<span data-ttu-id="be779-128">[scoredEmailAddress](scoredemailaddress.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be779-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="be779-129">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="be779-129">The person's email addresses.</span></span>|
|<span data-ttu-id="be779-130">givenName</span><span class="sxs-lookup"><span data-stu-id="be779-130">givenName</span></span>|<span data-ttu-id="be779-131">String</span><span class="sxs-lookup"><span data-stu-id="be779-131">String</span></span>|<span data-ttu-id="be779-132">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="be779-132">The person's given name.</span></span>|
|<span data-ttu-id="be779-133">id</span><span class="sxs-lookup"><span data-stu-id="be779-133">id</span></span>|<span data-ttu-id="be779-134">String</span><span class="sxs-lookup"><span data-stu-id="be779-134">String</span></span>|<span data-ttu-id="be779-p102">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="be779-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="be779-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="be779-137">imAddress</span></span>|<span data-ttu-id="be779-138">String</span><span class="sxs-lookup"><span data-stu-id="be779-138">String</span></span>|<span data-ttu-id="be779-p103">ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="be779-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="be779-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="be779-141">isFavorite</span></span>|<span data-ttu-id="be779-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="be779-142">Boolean</span></span>|<span data-ttu-id="be779-143">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="be779-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="be779-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="be779-144">jobTitle</span></span>|<span data-ttu-id="be779-145">String</span><span class="sxs-lookup"><span data-stu-id="be779-145">String</span></span>|<span data-ttu-id="be779-146">人物の役職。</span><span class="sxs-lookup"><span data-stu-id="be779-146">The person's job title.</span></span>|
|<span data-ttu-id="be779-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="be779-147">officeLocation</span></span>|<span data-ttu-id="be779-148">String</span><span class="sxs-lookup"><span data-stu-id="be779-148">String</span></span>|<span data-ttu-id="be779-149">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="be779-149">The location of the person's office.</span></span>|
|<span data-ttu-id="be779-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="be779-150">personNotes</span></span>|<span data-ttu-id="be779-151">String</span><span class="sxs-lookup"><span data-stu-id="be779-151">String</span></span>|<span data-ttu-id="be779-152">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="be779-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="be779-153">personType</span><span class="sxs-lookup"><span data-stu-id="be779-153">personType</span></span>|[<span data-ttu-id="be779-154">personType</span><span class="sxs-lookup"><span data-stu-id="be779-154">personType</span></span>](persontype.md) |<span data-ttu-id="be779-155">人物の種類。</span><span class="sxs-lookup"><span data-stu-id="be779-155">The type of person.</span></span>|
|<span data-ttu-id="be779-156">phones</span><span class="sxs-lookup"><span data-stu-id="be779-156">phones</span></span>|<span data-ttu-id="be779-157">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be779-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="be779-158">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="be779-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="be779-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="be779-159">postalAddresses</span></span>|<span data-ttu-id="be779-160">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be779-160">[location](location.md) collection</span></span>|<span data-ttu-id="be779-161">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="be779-161">The person's addresses.</span></span>|
|<span data-ttu-id="be779-162">profession</span><span class="sxs-lookup"><span data-stu-id="be779-162">profession</span></span>|<span data-ttu-id="be779-163">String</span><span class="sxs-lookup"><span data-stu-id="be779-163">String</span></span>|<span data-ttu-id="be779-164">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="be779-164">The person's profession.</span></span>|
|<span data-ttu-id="be779-165">surname</span><span class="sxs-lookup"><span data-stu-id="be779-165">surname</span></span>|<span data-ttu-id="be779-166">String</span><span class="sxs-lookup"><span data-stu-id="be779-166">String</span></span>|<span data-ttu-id="be779-167">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="be779-167">The person's surname.</span></span>|
|<span data-ttu-id="be779-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="be779-168">userPrincipalName</span></span>|<span data-ttu-id="be779-169">String</span><span class="sxs-lookup"><span data-stu-id="be779-169">String</span></span>|<span data-ttu-id="be779-p104">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="be779-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="be779-174">websites</span><span class="sxs-lookup"><span data-stu-id="be779-174">websites</span></span>|<span data-ttu-id="be779-175">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="be779-175">[website](website.md) collection</span></span>|<span data-ttu-id="be779-176">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="be779-176">The person's websites.</span></span>|
|<span data-ttu-id="be779-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="be779-177">yomiCompany</span></span>|<span data-ttu-id="be779-178">String</span><span class="sxs-lookup"><span data-stu-id="be779-178">String</span></span>|<span data-ttu-id="be779-179">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="be779-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be779-180">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be779-180">Relationships</span></span>

<span data-ttu-id="be779-181">なし。</span><span class="sxs-lookup"><span data-stu-id="be779-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be779-182">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be779-182">JSON representation</span></span>

<span data-ttu-id="be779-183">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be779-183">The following is a JSON representation of the resource.</span></span>

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
