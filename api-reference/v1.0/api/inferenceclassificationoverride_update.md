# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="6421a-101">inferenceClassificationOverride を更新する</span><span class="sxs-lookup"><span data-stu-id="6421a-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="6421a-102">指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。</span><span class="sxs-lookup"><span data-stu-id="6421a-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="6421a-103">[InferenceClassicationOverride](../resources/inferenceClassificationOverride.md) インスタンスのその他のフィールドの変更には、PATCH を使用できません。</span><span class="sxs-lookup"><span data-stu-id="6421a-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="6421a-104">送信者にオーバーライドがあり、その送信者が表示名を変更すると、既存のオーバーライドで [POST](inferenceclassification_post_overrides.md) を使用して [名前] フィールドの更新を実施できます。</span><span class="sxs-lookup"><span data-stu-id="6421a-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="6421a-105">送信者にオーバーライドがあり、その送信者が SMTP アドレスを変更すると、既存のオーバーライドを[削除](inferenceclassificationoverride_delete.md)して、新しい SMTP アドレスで新しくオーバーライドを[作成](inferenceclassification_post_overrides.md)することが、この送信者のオーバーライドを「更新」する唯一の方法になります。</span><span class="sxs-lookup"><span data-stu-id="6421a-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="6421a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6421a-106">Permissions</span></span>
<span data-ttu-id="6421a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6421a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6421a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6421a-109">Permission type</span></span>      | <span data-ttu-id="6421a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6421a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6421a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6421a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6421a-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6421a-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6421a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6421a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6421a-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6421a-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6421a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6421a-115">Application</span></span> | <span data-ttu-id="6421a-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6421a-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6421a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6421a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6421a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6421a-118">Request headers</span></span>
| <span data-ttu-id="6421a-119">名前</span><span class="sxs-lookup"><span data-stu-id="6421a-119">Name</span></span>       | <span data-ttu-id="6421a-120">型</span><span class="sxs-lookup"><span data-stu-id="6421a-120">Type</span></span> | <span data-ttu-id="6421a-121">説明</span><span class="sxs-lookup"><span data-stu-id="6421a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6421a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6421a-122">Authorization</span></span>  | <span data-ttu-id="6421a-123">string</span><span class="sxs-lookup"><span data-stu-id="6421a-123">string</span></span>  | <span data-ttu-id="6421a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6421a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6421a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6421a-126">Content-Type</span></span> | <span data-ttu-id="6421a-127">string</span><span class="sxs-lookup"><span data-stu-id="6421a-127">string</span></span>  | <span data-ttu-id="6421a-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="6421a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6421a-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="6421a-130">Request body</span></span>
<span data-ttu-id="6421a-p104">要求の本文内に、**classifyAs** の新しい値を指定します。最適なパフォーマンスを得るためには、変更されない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6421a-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="6421a-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6421a-133">Property</span></span>     | <span data-ttu-id="6421a-134">型</span><span class="sxs-lookup"><span data-stu-id="6421a-134">Type</span></span>   |<span data-ttu-id="6421a-135">説明</span><span class="sxs-lookup"><span data-stu-id="6421a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6421a-136">classifyAs</span><span class="sxs-lookup"><span data-stu-id="6421a-136">classifyAs</span></span>|<span data-ttu-id="6421a-137">string</span><span class="sxs-lookup"><span data-stu-id="6421a-137">string</span></span>| <span data-ttu-id="6421a-p105">特定の差出人からの着信メッセージを常時分類する方法を指定します。可能な値は、`focused`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="6421a-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="6421a-140">応答</span><span class="sxs-lookup"><span data-stu-id="6421a-140">Response</span></span>

<span data-ttu-id="6421a-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6421a-141">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6421a-142">例</span><span class="sxs-lookup"><span data-stu-id="6421a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6421a-143">要求</span><span class="sxs-lookup"><span data-stu-id="6421a-143">Request</span></span>
<span data-ttu-id="6421a-144">以下の例は、SMTP アドレス randiw@adatum.onmicrosoft.com のオーバーライドのものであり、`other` から `focused` に変更します。</span><span class="sxs-lookup"><span data-stu-id="6421a-144">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="6421a-145">応答</span><span class="sxs-lookup"><span data-stu-id="6421a-145">Response</span></span>
<span data-ttu-id="6421a-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6421a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->