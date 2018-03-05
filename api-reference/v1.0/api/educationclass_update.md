# <a name="update-educationclass-properties"></a><span data-ttu-id="26c43-101">educationclass プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="26c43-101">Update educationclass properties</span></span>

<span data-ttu-id="26c43-102">クラスのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="26c43-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="26c43-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26c43-103">Permissions</span></span>
<span data-ttu-id="26c43-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26c43-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26c43-106">Permission type</span></span>      | <span data-ttu-id="26c43-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26c43-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26c43-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26c43-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="26c43-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26c43-109">Not supported.</span></span>  |
|<span data-ttu-id="26c43-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26c43-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26c43-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26c43-111">Not supported.</span></span>   |
|<span data-ttu-id="26c43-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26c43-112">Application</span></span> | <span data-ttu-id="26c43-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c43-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="26c43-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26c43-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26c43-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26c43-115">Request headers</span></span>
| <span data-ttu-id="26c43-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26c43-116">Header</span></span>       | <span data-ttu-id="26c43-117">値</span><span class="sxs-lookup"><span data-stu-id="26c43-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26c43-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="26c43-118">Authorization</span></span>  | <span data-ttu-id="26c43-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26c43-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26c43-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26c43-121">Content-Type</span></span>  | <span data-ttu-id="26c43-122">application/json</span><span class="sxs-lookup"><span data-stu-id="26c43-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26c43-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="26c43-123">Request body</span></span>
<span data-ttu-id="26c43-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="26c43-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="26c43-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="26c43-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26c43-126">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="26c43-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26c43-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26c43-127">Property</span></span>     | <span data-ttu-id="26c43-128">型</span><span class="sxs-lookup"><span data-stu-id="26c43-128">Type</span></span>   |<span data-ttu-id="26c43-129">説明</span><span class="sxs-lookup"><span data-stu-id="26c43-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26c43-130">description</span><span class="sxs-lookup"><span data-stu-id="26c43-130">description</span></span>|<span data-ttu-id="26c43-131">String</span><span class="sxs-lookup"><span data-stu-id="26c43-131">String</span></span>| <span data-ttu-id="26c43-132">クラスの説明。</span><span class="sxs-lookup"><span data-stu-id="26c43-132">Description of the template.</span></span>|
|<span data-ttu-id="26c43-133">displayName</span><span class="sxs-lookup"><span data-stu-id="26c43-133">displayName</span></span>|<span data-ttu-id="26c43-134">String</span><span class="sxs-lookup"><span data-stu-id="26c43-134">String</span></span>| <span data-ttu-id="26c43-135">クラスの名前。</span><span class="sxs-lookup"><span data-stu-id="26c43-135">Name of the class.</span></span>|
|<span data-ttu-id="26c43-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="26c43-136">mailNickname</span></span>|<span data-ttu-id="26c43-137">String</span><span class="sxs-lookup"><span data-stu-id="26c43-137">String</span></span>| <span data-ttu-id="26c43-138">機能が有効になっている場合に、すべてのユーザーに電子メールを送信する電子メールのエイリアス。</span><span class="sxs-lookup"><span data-stu-id="26c43-138">Email alias for sending email to all users if that feature is enabled.</span></span> |
<!-- Please verify the revised description here. -->
<span data-ttu-id="26c43-139">|classCode|String| 学校が使用するクラス コード。| |externalId|String| 同期システムからのクラスの ID。</span><span class="sxs-lookup"><span data-stu-id="26c43-139">|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="26c43-140">| |externalName|String|同期システム内のクラスの名前。| |externalSource|string| このクラスを作成した方法。</span><span class="sxs-lookup"><span data-stu-id="26c43-140">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="26c43-141">使用可能な値: `sis`、`manual`、`enum_sentinel`.|</span><span class="sxs-lookup"><span data-stu-id="26c43-141">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>

## <a name="response"></a><span data-ttu-id="26c43-142">応答</span><span class="sxs-lookup"><span data-stu-id="26c43-142">Response</span></span>
<span data-ttu-id="26c43-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26c43-143">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26c43-144">例</span><span class="sxs-lookup"><span data-stu-id="26c43-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26c43-145">要求</span><span class="sxs-lookup"><span data-stu-id="26c43-145">Request</span></span>
<span data-ttu-id="26c43-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26c43-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/11014
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="26c43-147">応答</span><span class="sxs-lookup"><span data-stu-id="26c43-147">Response</span></span>
<span data-ttu-id="26c43-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26c43-148">The following is an example of the response.</span></span> 

><span data-ttu-id="26c43-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="26c43-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->