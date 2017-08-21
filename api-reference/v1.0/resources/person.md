# <a name="person-resource-type"></a><span data-ttu-id="4fb95-101">person リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fb95-101">person resource type</span></span>

<span data-ttu-id="4fb95-p101">メール、連絡先、ソーシャル ネットワークからの、人物に関する情報の集約です。人物は、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 連絡した人などになります。</span><span class="sxs-lookup"><span data-stu-id="4fb95-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="4fb95-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb95-104">Methods</span></span>

| <span data-ttu-id="4fb95-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb95-105">Method</span></span>           | <span data-ttu-id="4fb95-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fb95-106">Return Type</span></span>    |<span data-ttu-id="4fb95-107">説明</span><span class="sxs-lookup"><span data-stu-id="4fb95-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4fb95-108">ユーザーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4fb95-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="4fb95-109">**人物**</span><span class="sxs-lookup"><span data-stu-id="4fb95-109">**Person**</span></span> |<span data-ttu-id="4fb95-110">[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。</span><span class="sxs-lookup"><span data-stu-id="4fb95-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|
|[<span data-ttu-id="4fb95-111">人物を取得する</span><span class="sxs-lookup"><span data-stu-id="4fb95-111">Get person</span></span>](../api/person_get.md) | <span data-ttu-id="4fb95-112">**人物**</span><span class="sxs-lookup"><span data-stu-id="4fb95-112">**Person**</span></span> |<span data-ttu-id="4fb95-113">person オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="4fb95-113">Get the properties and relationships of a device object.</span></span>|


## <a name="properties"></a><span data-ttu-id="4fb95-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb95-114">Properties</span></span>
| <span data-ttu-id="4fb95-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb95-115">Property</span></span>     | <span data-ttu-id="4fb95-116">型</span><span class="sxs-lookup"><span data-stu-id="4fb95-116">Type</span></span>   |<span data-ttu-id="4fb95-117">説明</span><span class="sxs-lookup"><span data-stu-id="4fb95-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fb95-118">birthday</span><span class="sxs-lookup"><span data-stu-id="4fb95-118">birthday</span></span>|<span data-ttu-id="4fb95-119">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-119">String</span></span>|<span data-ttu-id="4fb95-120">人物の誕生日。</span><span class="sxs-lookup"><span data-stu-id="4fb95-120">The person's birthday.</span></span>|
|<span data-ttu-id="4fb95-121">companyName</span><span class="sxs-lookup"><span data-stu-id="4fb95-121">companyName</span></span>|<span data-ttu-id="4fb95-122">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-122">String</span></span>|<span data-ttu-id="4fb95-123">人物の会社名。</span><span class="sxs-lookup"><span data-stu-id="4fb95-123">The name of the contact's company.</span></span>|
|<span data-ttu-id="4fb95-124">department</span><span class="sxs-lookup"><span data-stu-id="4fb95-124">department</span></span>|<span data-ttu-id="4fb95-125">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-125">String</span></span>|<span data-ttu-id="4fb95-126">人物の部署。</span><span class="sxs-lookup"><span data-stu-id="4fb95-126">The person's department.</span></span>|
|<span data-ttu-id="4fb95-127">displayName</span><span class="sxs-lookup"><span data-stu-id="4fb95-127">displayName</span></span>|<span data-ttu-id="4fb95-128">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-128">String</span></span>|<span data-ttu-id="4fb95-129">人物の表示名。</span><span class="sxs-lookup"><span data-stu-id="4fb95-129">The person's display name.</span></span>|
|<span data-ttu-id="4fb95-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="4fb95-130">scoredEmailAddresses</span></span>|<span data-ttu-id="4fb95-131">[scoredEmailAddress](scoredemailaddress.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb95-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="4fb95-132">人物の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="4fb95-132">The contact's email addresses.</span></span>|
|<span data-ttu-id="4fb95-133">givenName</span><span class="sxs-lookup"><span data-stu-id="4fb95-133">givenName</span></span>|<span data-ttu-id="4fb95-134">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-134">String</span></span>|<span data-ttu-id="4fb95-135">人物に指定された名前。</span><span class="sxs-lookup"><span data-stu-id="4fb95-135">The contact's given name.</span></span>|
|<span data-ttu-id="4fb95-136">id</span><span class="sxs-lookup"><span data-stu-id="4fb95-136">id</span></span>|<span data-ttu-id="4fb95-137">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-137">String</span></span>|<span data-ttu-id="4fb95-p102">人物の一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb95-p102">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="4fb95-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="4fb95-140">IMAddress</span></span>|<span data-ttu-id="4fb95-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb95-141">String collection</span></span>|<span data-ttu-id="4fb95-p103">ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb95-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.</span></span>|
|<span data-ttu-id="4fb95-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="4fb95-144">isFavorite</span></span>|<span data-ttu-id="4fb95-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb95-145">Boolean</span></span>|<span data-ttu-id="4fb95-146">ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。</span><span class="sxs-lookup"><span data-stu-id="4fb95-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="4fb95-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="4fb95-147">jobTitle</span></span>|<span data-ttu-id="4fb95-148">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-148">String</span></span>|<span data-ttu-id="4fb95-149">人物の役職。</span><span class="sxs-lookup"><span data-stu-id="4fb95-149">The contact's job title.</span></span>|
|<span data-ttu-id="4fb95-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="4fb95-150">officeLocation</span></span>|<span data-ttu-id="4fb95-151">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-151">String</span></span>|<span data-ttu-id="4fb95-152">人物のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="4fb95-152">The location of the contact's office.</span></span>|
|<span data-ttu-id="4fb95-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="4fb95-153">personNotes</span></span>|<span data-ttu-id="4fb95-154">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-154">String</span></span>|<span data-ttu-id="4fb95-155">ユーザーがこの人物について記入した自由形式のメモ。</span><span class="sxs-lookup"><span data-stu-id="4fb95-155">Free-form notes that the the user has taken about this person.</span></span>|
|<span data-ttu-id="4fb95-156">personType</span><span class="sxs-lookup"><span data-stu-id="4fb95-156">personType</span></span>|<span data-ttu-id="4fb95-157">[personType](persontype.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb95-157">[personType](persontype.md) collection</span></span>|<span data-ttu-id="4fb95-158">人物の種類。</span><span class="sxs-lookup"><span data-stu-id="4fb95-158">The type of person.</span></span>|
|<span data-ttu-id="4fb95-159">phones</span><span class="sxs-lookup"><span data-stu-id="4fb95-159">Phones</span></span>|<span data-ttu-id="4fb95-160">[phone](phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb95-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="4fb95-161">人物の電話番号。</span><span class="sxs-lookup"><span data-stu-id="4fb95-161">The user's phone numbers.</span></span>|
|<span data-ttu-id="4fb95-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="4fb95-162">PostalAddresses</span></span>|<span data-ttu-id="4fb95-163">[location](location.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb95-163">[location](location.md) collection</span></span>|<span data-ttu-id="4fb95-164">人物のアドレス。</span><span class="sxs-lookup"><span data-stu-id="4fb95-164">The person's addresses.</span></span>|
|<span data-ttu-id="4fb95-165">profession</span><span class="sxs-lookup"><span data-stu-id="4fb95-165">profession</span></span>|<span data-ttu-id="4fb95-166">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-166">String</span></span>|<span data-ttu-id="4fb95-167">人物の職業。</span><span class="sxs-lookup"><span data-stu-id="4fb95-167">The person's profession.</span></span>|
|<span data-ttu-id="4fb95-168">surname</span><span class="sxs-lookup"><span data-stu-id="4fb95-168">surname</span></span>|<span data-ttu-id="4fb95-169">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-169">String</span></span>|<span data-ttu-id="4fb95-170">人物の姓。</span><span class="sxs-lookup"><span data-stu-id="4fb95-170">The person's surname.</span></span>|
|<span data-ttu-id="4fb95-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fb95-171">userPrincipalName</span></span>|<span data-ttu-id="4fb95-172">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-172">String</span></span>|<span data-ttu-id="4fb95-p104">人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。</span><span class="sxs-lookup"><span data-stu-id="4fb95-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="4fb95-177">websites</span><span class="sxs-lookup"><span data-stu-id="4fb95-177">Websites</span></span>|<span data-ttu-id="4fb95-178">[website](website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb95-178">[website](website.md) collection</span></span>|<span data-ttu-id="4fb95-179">人物の Web サイト。</span><span class="sxs-lookup"><span data-stu-id="4fb95-179">The person's websites.</span></span>|
|<span data-ttu-id="4fb95-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="4fb95-180">yomiCompany</span></span>|<span data-ttu-id="4fb95-181">String</span><span class="sxs-lookup"><span data-stu-id="4fb95-181">String</span></span>|<span data-ttu-id="4fb95-182">人物の会社の日本名の読み仮名。</span><span class="sxs-lookup"><span data-stu-id="4fb95-182">The phonetic Japanese company name of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fb95-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fb95-183">Relationships</span></span>
<span data-ttu-id="4fb95-184">なし。</span><span class="sxs-lookup"><span data-stu-id="4fb95-184">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4fb95-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fb95-185">JSON representation</span></span>

<span data-ttu-id="4fb95-186">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4fb95-186">Here is a JSON representation of the resource</span></span>

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
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredemailaddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": [{"@odata.type": "microsoft.graph.persontype"}],
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
