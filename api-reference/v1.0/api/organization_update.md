# <a name="update-organization"></a><span data-ttu-id="ddfd9-101">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="ddfd9-101">Update organization</span></span>

<span data-ttu-id="ddfd9-102">現在認証されている組織のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddfd9-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ddfd9-103">Permissions</span></span>

<span data-ttu-id="ddfd9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ddfd9-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ddfd9-106">Permission type</span></span> | <span data-ttu-id="ddfd9-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ddfd9-107">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddfd9-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ddfd9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ddfd9-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddfd9-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddfd9-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ddfd9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddfd9-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-111">Not supported.</span></span>    |
|<span data-ttu-id="ddfd9-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ddfd9-112">Application</span></span> | <span data-ttu-id="ddfd9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddfd9-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ddfd9-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="ddfd9-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ddfd9-115">Request headers</span></span>

| <span data-ttu-id="ddfd9-116">名前</span><span class="sxs-lookup"><span data-stu-id="ddfd9-116">Name</span></span>       | <span data-ttu-id="ddfd9-117">型</span><span class="sxs-lookup"><span data-stu-id="ddfd9-117">Type</span></span> | <span data-ttu-id="ddfd9-118">説明</span><span class="sxs-lookup"><span data-stu-id="ddfd9-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddfd9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddfd9-119">Authorization</span></span>  | <span data-ttu-id="ddfd9-120">string</span><span class="sxs-lookup"><span data-stu-id="ddfd9-120">string</span></span>  | <span data-ttu-id="ddfd9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddfd9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ddfd9-123">Request body</span></span>
<span data-ttu-id="ddfd9-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ddfd9-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ddfd9-126">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ddfd9-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddfd9-127">Property</span></span>     | <span data-ttu-id="ddfd9-128">型</span><span class="sxs-lookup"><span data-stu-id="ddfd9-128">Type</span></span>   |<span data-ttu-id="ddfd9-129">説明</span><span class="sxs-lookup"><span data-stu-id="ddfd9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddfd9-130">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="ddfd9-130">marketingNotificationEmails</span></span>|<span data-ttu-id="ddfd9-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ddfd9-131">String collection</span></span>|                                        <span data-ttu-id="ddfd9-132">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-132">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ddfd9-133">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="ddfd9-133">privacyProfile</span></span>|[<span data-ttu-id="ddfd9-134">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="ddfd9-134">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="ddfd9-135">組織のプライバシー プロファイル (statementUrl と contactEmail を設定します)。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-135">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="ddfd9-136">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="ddfd9-136">securityComplianceNotificationMails</span></span>|<span data-ttu-id="ddfd9-137">String collection</span><span class="sxs-lookup"><span data-stu-id="ddfd9-137">String collection</span></span>||
|<span data-ttu-id="ddfd9-138">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="ddfd9-138">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="ddfd9-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ddfd9-139">String collection</span></span>||
|<span data-ttu-id="ddfd9-140">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="ddfd9-140">technicalNotificationMails</span></span>|<span data-ttu-id="ddfd9-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ddfd9-141">String collection</span></span>|                                        <span data-ttu-id="ddfd9-142">**注**: Null は許容されません。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-142">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="ddfd9-143">応答</span><span class="sxs-lookup"><span data-stu-id="ddfd9-143">Response</span></span>

<span data-ttu-id="ddfd9-144">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ddfd9-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ddfd9-145">例</span><span class="sxs-lookup"><span data-stu-id="ddfd9-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddfd9-146">要求</span><span class="sxs-lookup"><span data-stu-id="ddfd9-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="ddfd9-147">応答</span><span class="sxs-lookup"><span data-stu-id="ddfd9-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
