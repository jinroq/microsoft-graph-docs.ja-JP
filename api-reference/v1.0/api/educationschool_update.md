# <a name="update-educationschool-properties"></a><span data-ttu-id="ccbd3-101">educationschool プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="ccbd3-101">Update educationschool properties</span></span>

<span data-ttu-id="ccbd3-102">学校オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-102">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccbd3-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ccbd3-103">Permissions</span></span>
<span data-ttu-id="ccbd3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ccbd3-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ccbd3-106">Permission type</span></span>      | <span data-ttu-id="ccbd3-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ccbd3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccbd3-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ccbd3-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="ccbd3-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-109">Not supported.</span></span>  |
|<span data-ttu-id="ccbd3-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ccbd3-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ccbd3-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-111">Not supported.</span></span>  |
|<span data-ttu-id="ccbd3-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ccbd3-112">Application</span></span> | <span data-ttu-id="ccbd3-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccbd3-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccbd3-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ccbd3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ccbd3-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ccbd3-115">Request headers</span></span>
| <span data-ttu-id="ccbd3-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ccbd3-116">Header</span></span>       | <span data-ttu-id="ccbd3-117">値</span><span class="sxs-lookup"><span data-stu-id="ccbd3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ccbd3-118">承認</span><span class="sxs-lookup"><span data-stu-id="ccbd3-118">Authorization</span></span>  | <span data-ttu-id="ccbd3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ccbd3-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccbd3-121">Content-Type</span></span>  | <span data-ttu-id="ccbd3-122">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="ccbd3-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ccbd3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ccbd3-123">Request body</span></span>
<span data-ttu-id="ccbd3-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ccbd3-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ccbd3-126">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ccbd3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccbd3-127">Property</span></span>     | <span data-ttu-id="ccbd3-128">タイプ</span><span class="sxs-lookup"><span data-stu-id="ccbd3-128">Type</span></span>   |<span data-ttu-id="ccbd3-129">説明</span><span class="sxs-lookup"><span data-stu-id="ccbd3-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccbd3-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ccbd3-130">displayName</span></span>| <span data-ttu-id="ccbd3-131">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-131">String</span></span>| <span data-ttu-id="ccbd3-132">学校の表示名</span><span class="sxs-lookup"><span data-stu-id="ccbd3-132">Display name of the school</span></span>| 
|<span data-ttu-id="ccbd3-133">description</span><span class="sxs-lookup"><span data-stu-id="ccbd3-133">description</span></span>| <span data-ttu-id="ccbd3-134">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-134">String</span></span> | <span data-ttu-id="ccbd3-135">学校の説明</span><span class="sxs-lookup"><span data-stu-id="ccbd3-135">Description of the school</span></span>| 
|<span data-ttu-id="ccbd3-136">principalEmail</span><span class="sxs-lookup"><span data-stu-id="ccbd3-136">principalEmail</span></span>| <span data-ttu-id="ccbd3-137">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-137">String</span></span>| <span data-ttu-id="ccbd3-138">プリンシパルの電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="ccbd3-138">Email address of the principal</span></span>|
|<span data-ttu-id="ccbd3-139">principalName</span><span class="sxs-lookup"><span data-stu-id="ccbd3-139">principalName</span></span>| <span data-ttu-id="ccbd3-140">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-140">String</span></span> | <span data-ttu-id="ccbd3-141">プリンシパルの名前</span><span class="sxs-lookup"><span data-stu-id="ccbd3-141">Name of the principal</span></span>|
|<span data-ttu-id="ccbd3-142">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="ccbd3-142">externalPrincipalId</span></span>| <span data-ttu-id="ccbd3-143">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-143">String</span></span> | <span data-ttu-id="ccbd3-144">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-144">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="ccbd3-145">highestGrade</span><span class="sxs-lookup"><span data-stu-id="ccbd3-145">highestGrade</span></span>|<span data-ttu-id="ccbd3-146">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-146">String</span></span>| <span data-ttu-id="ccbd3-147">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-147">Highest grade taught.</span></span> |
|<span data-ttu-id="ccbd3-148">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="ccbd3-148">lowestGrade</span></span>|<span data-ttu-id="ccbd3-149">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-149">String</span></span>| <span data-ttu-id="ccbd3-150">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-150">Lowest grade taught.</span></span> |
|<span data-ttu-id="ccbd3-151">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="ccbd3-151">schoolNumber</span></span>|<span data-ttu-id="ccbd3-152">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-152">String</span></span>| <span data-ttu-id="ccbd3-153">学校番号。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-153">School Number.</span></span>|
|<span data-ttu-id="ccbd3-154">externalId</span><span class="sxs-lookup"><span data-stu-id="ccbd3-154">externalId</span></span>|<span data-ttu-id="ccbd3-155">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-155">String</span></span>| <span data-ttu-id="ccbd3-156">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-156">Id of school in syncing system.</span></span> |
|<span data-ttu-id="ccbd3-157">phone</span><span class="sxs-lookup"><span data-stu-id="ccbd3-157">phone</span></span>|<span data-ttu-id="ccbd3-158">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-158">String</span></span>| <span data-ttu-id="ccbd3-159">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-159">Phone number of school.</span></span> |
|<span data-ttu-id="ccbd3-160">fax</span><span class="sxs-lookup"><span data-stu-id="ccbd3-160">fax</span></span>|<span data-ttu-id="ccbd3-161">String</span><span class="sxs-lookup"><span data-stu-id="ccbd3-161">String</span></span>| <span data-ttu-id="ccbd3-162">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-162">Fax number of school.</span></span> |
|<span data-ttu-id="ccbd3-163">address</span><span class="sxs-lookup"><span data-stu-id="ccbd3-163">address</span></span>|[<span data-ttu-id="ccbd3-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="ccbd3-164">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="ccbd3-165">学校のアドレス。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-165">Address of the School.</span></span>|
|<span data-ttu-id="ccbd3-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="ccbd3-166">createdBy</span></span>|[<span data-ttu-id="ccbd3-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="ccbd3-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ccbd3-168">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-168">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="ccbd3-169">応答</span><span class="sxs-lookup"><span data-stu-id="ccbd3-169">Response</span></span>
<span data-ttu-id="ccbd3-170">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-170">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ccbd3-171">例</span><span class="sxs-lookup"><span data-stu-id="ccbd3-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccbd3-172">要求</span><span class="sxs-lookup"><span data-stu-id="ccbd3-172">Request</span></span>
<span data-ttu-id="ccbd3-173">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="ccbd3-174">応答</span><span class="sxs-lookup"><span data-stu-id="ccbd3-174">Response</span></span>
<span data-ttu-id="ccbd3-175">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-175">The following is an example of the response.</span></span> 

><span data-ttu-id="ccbd3-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ccbd3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
