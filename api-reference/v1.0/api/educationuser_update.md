# <a name="update-educationuser-properties"></a><span data-ttu-id="2610b-101">educationUser プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="2610b-101">Update educationUser properties</span></span>

<span data-ttu-id="2610b-102">**educationuser** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2610b-102">Update the properties of an **eventMessage** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2610b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2610b-103">Permissions</span></span>
<span data-ttu-id="2610b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2610b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2610b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2610b-106">Permission type</span></span>      | <span data-ttu-id="2610b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2610b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2610b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2610b-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="2610b-109">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2610b-109">Not supported.</span></span>  |
|<span data-ttu-id="2610b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2610b-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2610b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2610b-111">Not supported.</span></span>  |
|<span data-ttu-id="2610b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2610b-112">Application</span></span> | <span data-ttu-id="2610b-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2610b-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2610b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2610b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2610b-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2610b-115">Request headers</span></span>
| <span data-ttu-id="2610b-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2610b-116">Header</span></span>       | <span data-ttu-id="2610b-117">値</span><span class="sxs-lookup"><span data-stu-id="2610b-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2610b-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2610b-118">Authorization</span></span>  | <span data-ttu-id="2610b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2610b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2610b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2610b-121">Content-Type</span></span>  | <span data-ttu-id="2610b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2610b-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2610b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2610b-123">Request body</span></span>
<span data-ttu-id="2610b-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2610b-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2610b-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="2610b-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2610b-126">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2610b-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2610b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2610b-127">Property</span></span>     | <span data-ttu-id="2610b-128">型</span><span class="sxs-lookup"><span data-stu-id="2610b-128">Type</span></span>   |<span data-ttu-id="2610b-129">説明</span><span class="sxs-lookup"><span data-stu-id="2610b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2610b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2610b-130">displayName</span></span>| <span data-ttu-id="2610b-131">String</span><span class="sxs-lookup"><span data-stu-id="2610b-131">String</span></span>| <span data-ttu-id="2610b-132">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="2610b-132">Display Name of User</span></span>|
|<span data-ttu-id="2610b-133">givenName</span><span class="sxs-lookup"><span data-stu-id="2610b-133">givenName</span></span>| <span data-ttu-id="2610b-134">String</span><span class="sxs-lookup"><span data-stu-id="2610b-134">String</span></span> | <span data-ttu-id="2610b-135">名</span><span class="sxs-lookup"><span data-stu-id="2610b-135">First Name</span></span> |
|<span data-ttu-id="2610b-136">middleName</span><span class="sxs-lookup"><span data-stu-id="2610b-136">middleName</span></span>| <span data-ttu-id="2610b-137">String</span><span class="sxs-lookup"><span data-stu-id="2610b-137">String</span></span> | <span data-ttu-id="2610b-138">ユーザーのミドル ネーム</span><span class="sxs-lookup"><span data-stu-id="2610b-138">Middle Name of user</span></span>|
|<span data-ttu-id="2610b-139">surname</span><span class="sxs-lookup"><span data-stu-id="2610b-139">surname</span></span>| <span data-ttu-id="2610b-140">String</span><span class="sxs-lookup"><span data-stu-id="2610b-140">String</span></span> | <span data-ttu-id="2610b-141">ユーザーの姓</span><span class="sxs-lookup"><span data-stu-id="2610b-141">Surname of user</span></span>|
|<span data-ttu-id="2610b-142">mail</span><span class="sxs-lookup"><span data-stu-id="2610b-142">mail</span></span>| <span data-ttu-id="2610b-143">String</span><span class="sxs-lookup"><span data-stu-id="2610b-143">String</span></span>| <span data-ttu-id="2610b-144">メール アドレス</span><span class="sxs-lookup"><span data-stu-id="2610b-144">Email Address</span></span>|
|<span data-ttu-id="2610b-145">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2610b-145">mobilePhone</span></span>| <span data-ttu-id="2610b-146">String</span><span class="sxs-lookup"><span data-stu-id="2610b-146">String</span></span> | <span data-ttu-id="2610b-147">ユーザーの携帯電話番号</span><span class="sxs-lookup"><span data-stu-id="2610b-147">Mobile number of user</span></span> |
|<span data-ttu-id="2610b-148">externalSource</span><span class="sxs-lookup"><span data-stu-id="2610b-148">externalSource</span></span>|<span data-ttu-id="2610b-149">string</span><span class="sxs-lookup"><span data-stu-id="2610b-149">string</span></span>| <span data-ttu-id="2610b-150">使用可能な値: `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="2610b-150">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2610b-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="2610b-151">externalSource</span></span>|<span data-ttu-id="2610b-152">string</span><span class="sxs-lookup"><span data-stu-id="2610b-152">string</span></span>| <span data-ttu-id="2610b-153">このユーザーが作成された場所。</span><span class="sxs-lookup"><span data-stu-id="2610b-153">Where this user was created from.</span></span>  <span data-ttu-id="2610b-154">使用可能な値: `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="2610b-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2610b-155">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="2610b-155">MailingAddress</span></span>|[<span data-ttu-id="2610b-156">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2610b-156">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="2610b-157">ユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2610b-157">Mail address of user.</span></span>|
|<span data-ttu-id="2610b-158">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="2610b-158">residenceAddress</span></span>|[<span data-ttu-id="2610b-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2610b-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="2610b-160">ユーザーが在住している場所のアドレス。</span><span class="sxs-lookup"><span data-stu-id="2610b-160">Address where user lives.</span></span>|
|<span data-ttu-id="2610b-161">primaryRole</span><span class="sxs-lookup"><span data-stu-id="2610b-161">primaryRole</span></span>|<span data-ttu-id="2610b-162">string</span><span class="sxs-lookup"><span data-stu-id="2610b-162">string</span></span>| <span data-ttu-id="2610b-163">ユーザーの既定のロール。</span><span class="sxs-lookup"><span data-stu-id="2610b-163">Default Role for a user.</span></span>  <span data-ttu-id="2610b-164">ユーザーのロールは、個々のクラスで異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="2610b-164">The user's role might be different in an individual class.</span></span> <span data-ttu-id="2610b-165">使用可能な値: `student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="2610b-165">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2610b-166">student</span><span class="sxs-lookup"><span data-stu-id="2610b-166">student.</span></span>|[<span data-ttu-id="2610b-167">educationStudent</span><span class="sxs-lookup"><span data-stu-id="2610b-167">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="2610b-168">プライマリ ロールが学生の場合、このブロックには学生固有のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2610b-168">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="2610b-169">teacher</span><span class="sxs-lookup"><span data-stu-id="2610b-169">teacher</span></span>|[<span data-ttu-id="2610b-170">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="2610b-170">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="2610b-171">プライマリ ロールが教師の場合、このブロックには教師固有のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2610b-171">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="2610b-172">応答</span><span class="sxs-lookup"><span data-stu-id="2610b-172">Response</span></span>
<span data-ttu-id="2610b-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationUser](../resources/educationuser.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2610b-173">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2610b-174">例</span><span class="sxs-lookup"><span data-stu-id="2610b-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2610b-175">要求</span><span class="sxs-lookup"><span data-stu-id="2610b-175">Request</span></span>
<span data-ttu-id="2610b-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2610b-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a><span data-ttu-id="2610b-177">応答</span><span class="sxs-lookup"><span data-stu-id="2610b-177">Response</span></span>
<span data-ttu-id="2610b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2610b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->