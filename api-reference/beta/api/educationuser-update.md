---
title: educationUser プロパティを更新する
description: '**educationuser** オブジェクトのプロパティを更新します。'
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 117acfb747457986af3e615f1006a6de1ceefe0b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931185"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="18e89-103">educationUser プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="18e89-103">Update educationUser properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e89-104">**educationuser** オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18e89-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="18e89-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18e89-105">Permissions</span></span>
<span data-ttu-id="18e89-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18e89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e89-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18e89-108">Permission type</span></span>      | <span data-ttu-id="18e89-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18e89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18e89-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18e89-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="18e89-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18e89-111">Not supported.</span></span>  |
|<span data-ttu-id="18e89-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18e89-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18e89-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18e89-113">Not supported.</span></span>  |
|<span data-ttu-id="18e89-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18e89-114">Application</span></span> | <span data-ttu-id="18e89-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e89-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18e89-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18e89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="18e89-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18e89-117">Request headers</span></span>
| <span data-ttu-id="18e89-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18e89-118">Header</span></span>       | <span data-ttu-id="18e89-119">値</span><span class="sxs-lookup"><span data-stu-id="18e89-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18e89-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18e89-120">Authorization</span></span>  | <span data-ttu-id="18e89-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18e89-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18e89-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18e89-123">Content-Type</span></span>  | <span data-ttu-id="18e89-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18e89-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18e89-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="18e89-125">Request body</span></span>
<span data-ttu-id="18e89-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="18e89-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="18e89-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="18e89-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="18e89-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="18e89-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18e89-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18e89-129">Property</span></span>     | <span data-ttu-id="18e89-130">型</span><span class="sxs-lookup"><span data-stu-id="18e89-130">Type</span></span>   |<span data-ttu-id="18e89-131">説明</span><span class="sxs-lookup"><span data-stu-id="18e89-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18e89-132">displayName</span><span class="sxs-lookup"><span data-stu-id="18e89-132">displayName</span></span>| <span data-ttu-id="18e89-133">文字列</span><span class="sxs-lookup"><span data-stu-id="18e89-133">String</span></span>| <span data-ttu-id="18e89-134">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="18e89-134">Display Name of User</span></span>|
|<span data-ttu-id="18e89-135">givenName</span><span class="sxs-lookup"><span data-stu-id="18e89-135">givenName</span></span>| <span data-ttu-id="18e89-136">String</span><span class="sxs-lookup"><span data-stu-id="18e89-136">String</span></span> | <span data-ttu-id="18e89-137">名</span><span class="sxs-lookup"><span data-stu-id="18e89-137">First Name</span></span> |
|<span data-ttu-id="18e89-138">middleName</span><span class="sxs-lookup"><span data-stu-id="18e89-138">middleName</span></span>| <span data-ttu-id="18e89-139">String</span><span class="sxs-lookup"><span data-stu-id="18e89-139">String</span></span> | <span data-ttu-id="18e89-140">ユーザーのミドル ネーム</span><span class="sxs-lookup"><span data-stu-id="18e89-140">Middle Name of user</span></span>|
|<span data-ttu-id="18e89-141">surname</span><span class="sxs-lookup"><span data-stu-id="18e89-141">surname</span></span>| <span data-ttu-id="18e89-142">String</span><span class="sxs-lookup"><span data-stu-id="18e89-142">String</span></span> | <span data-ttu-id="18e89-143">ユーザーの姓</span><span class="sxs-lookup"><span data-stu-id="18e89-143">Surname of user</span></span>|
|<span data-ttu-id="18e89-144">mail</span><span class="sxs-lookup"><span data-stu-id="18e89-144">mail</span></span>| <span data-ttu-id="18e89-145">String</span><span class="sxs-lookup"><span data-stu-id="18e89-145">String</span></span>| <span data-ttu-id="18e89-146">メール アドレス</span><span class="sxs-lookup"><span data-stu-id="18e89-146">email address</span></span>|
|<span data-ttu-id="18e89-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="18e89-147">mobilePhone</span></span>| <span data-ttu-id="18e89-148">String</span><span class="sxs-lookup"><span data-stu-id="18e89-148">String</span></span> | <span data-ttu-id="18e89-149">ユーザーの携帯電話番号</span><span class="sxs-lookup"><span data-stu-id="18e89-149">Mobile number of user</span></span> |
|<span data-ttu-id="18e89-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="18e89-150">externalSource</span></span>|<span data-ttu-id="18e89-151">string</span><span class="sxs-lookup"><span data-stu-id="18e89-151">string</span></span>| <span data-ttu-id="18e89-152">可能な値は、`sis`、`manual`、`enum_sentinel` です。</span><span class="sxs-lookup"><span data-stu-id="18e89-152">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="18e89-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="18e89-153">externalSource</span></span>|<span data-ttu-id="18e89-154">string</span><span class="sxs-lookup"><span data-stu-id="18e89-154">string</span></span>| <span data-ttu-id="18e89-155">このユーザーが作成された場所。</span><span class="sxs-lookup"><span data-stu-id="18e89-155">Where this user was created from.</span></span>  <span data-ttu-id="18e89-156">可能な値は、`sis`、`manual`、`enum_sentinel` です。</span><span class="sxs-lookup"><span data-stu-id="18e89-156">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="18e89-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="18e89-157">mailingAddress</span></span>|[<span data-ttu-id="18e89-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="18e89-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="18e89-159">ユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="18e89-159">Mail address of user.</span></span>|
|<span data-ttu-id="18e89-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="18e89-160">residenceAddress</span></span>|[<span data-ttu-id="18e89-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="18e89-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="18e89-162">ユーザーが在住している場所のアドレス。</span><span class="sxs-lookup"><span data-stu-id="18e89-162">Address where user lives.</span></span>|
|<span data-ttu-id="18e89-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="18e89-163">primaryRole</span></span>|<span data-ttu-id="18e89-164">string</span><span class="sxs-lookup"><span data-stu-id="18e89-164">string</span></span>| <span data-ttu-id="18e89-165">ユーザーの既定のロール。</span><span class="sxs-lookup"><span data-stu-id="18e89-165">Default Role for a user.</span></span>  <span data-ttu-id="18e89-166">ユーザーのロールは、個々のクラスで異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="18e89-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="18e89-167">使用可能な値: `student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="18e89-167">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="18e89-168">student</span><span class="sxs-lookup"><span data-stu-id="18e89-168">student</span></span>|[<span data-ttu-id="18e89-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="18e89-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="18e89-170">プライマリ ロールが学生の場合、このブロックには学生固有のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="18e89-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="18e89-171">teacher</span><span class="sxs-lookup"><span data-stu-id="18e89-171">teacher</span></span>|[<span data-ttu-id="18e89-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="18e89-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="18e89-173">プライマリロールが教師の場合、このブロックには教師固有のデータが含まれます。</span><span class="sxs-lookup"><span data-stu-id="18e89-173">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="18e89-174">応答</span><span class="sxs-lookup"><span data-stu-id="18e89-174">Response</span></span>
<span data-ttu-id="18e89-175">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationUser](../resources/educationuser.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18e89-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18e89-176">例</span><span class="sxs-lookup"><span data-stu-id="18e89-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18e89-177">要求</span><span class="sxs-lookup"><span data-stu-id="18e89-177">Request</span></span>
<span data-ttu-id="18e89-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18e89-178">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18e89-179">プロトコル</span><span class="sxs-lookup"><span data-stu-id="18e89-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18e89-180">C#</span><span class="sxs-lookup"><span data-stu-id="18e89-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18e89-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="18e89-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18e89-182">目的-C</span><span class="sxs-lookup"><span data-stu-id="18e89-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18e89-183">Java</span><span class="sxs-lookup"><span data-stu-id="18e89-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18e89-184">応答</span><span class="sxs-lookup"><span data-stu-id="18e89-184">Response</span></span>
<span data-ttu-id="18e89-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18e89-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
