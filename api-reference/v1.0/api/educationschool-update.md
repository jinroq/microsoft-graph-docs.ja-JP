---
title: educationschool プロパティを更新する
description: 学校オブジェクトのプロパティを更新します。
ms.openlocfilehash: aa413360305b32f3e2c5288192929ae48279bd60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020397"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="511ae-103">educationschool プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="511ae-103">Update educationschool properties</span></span>

<span data-ttu-id="511ae-104">学校オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="511ae-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="511ae-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="511ae-105">Permissions</span></span>
<span data-ttu-id="511ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="511ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="511ae-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="511ae-108">Permission type</span></span>      | <span data-ttu-id="511ae-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="511ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="511ae-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="511ae-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="511ae-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="511ae-111">Not supported.</span></span>  |
|<span data-ttu-id="511ae-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="511ae-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="511ae-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="511ae-113">Not supported.</span></span>  |
|<span data-ttu-id="511ae-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="511ae-114">Application</span></span> | <span data-ttu-id="511ae-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="511ae-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="511ae-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="511ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="511ae-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="511ae-117">Request headers</span></span>
| <span data-ttu-id="511ae-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="511ae-118">Header</span></span>       | <span data-ttu-id="511ae-119">値</span><span class="sxs-lookup"><span data-stu-id="511ae-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="511ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="511ae-120">Authorization</span></span>  | <span data-ttu-id="511ae-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="511ae-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="511ae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="511ae-123">Content-Type</span></span>  | <span data-ttu-id="511ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="511ae-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="511ae-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="511ae-125">Request body</span></span>
<span data-ttu-id="511ae-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="511ae-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="511ae-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="511ae-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="511ae-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="511ae-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="511ae-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="511ae-129">Property</span></span>     | <span data-ttu-id="511ae-130">型</span><span class="sxs-lookup"><span data-stu-id="511ae-130">Type</span></span>   |<span data-ttu-id="511ae-131">説明</span><span class="sxs-lookup"><span data-stu-id="511ae-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="511ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="511ae-132">displayName</span></span>| <span data-ttu-id="511ae-133">String</span><span class="sxs-lookup"><span data-stu-id="511ae-133">String</span></span>| <span data-ttu-id="511ae-134">学校の表示名</span><span class="sxs-lookup"><span data-stu-id="511ae-134">Display name of the school</span></span>| 
|<span data-ttu-id="511ae-135">説明</span><span class="sxs-lookup"><span data-stu-id="511ae-135">description</span></span>| <span data-ttu-id="511ae-136">String</span><span class="sxs-lookup"><span data-stu-id="511ae-136">String</span></span> | <span data-ttu-id="511ae-137">学校の説明</span><span class="sxs-lookup"><span data-stu-id="511ae-137">Description of the school</span></span>| 
|<span data-ttu-id="511ae-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="511ae-138">principalEmail</span></span>| <span data-ttu-id="511ae-139">String</span><span class="sxs-lookup"><span data-stu-id="511ae-139">String</span></span>| <span data-ttu-id="511ae-140">プリンシパルの電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="511ae-140">Email address of the principal</span></span>|
|<span data-ttu-id="511ae-141">principalName</span><span class="sxs-lookup"><span data-stu-id="511ae-141">principalName</span></span>| <span data-ttu-id="511ae-142">String</span><span class="sxs-lookup"><span data-stu-id="511ae-142">String</span></span> | <span data-ttu-id="511ae-143">プリンシパルの名前</span><span class="sxs-lookup"><span data-stu-id="511ae-143">Name of the principal</span></span>|
|<span data-ttu-id="511ae-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="511ae-144">externalPrincipalId</span></span>| <span data-ttu-id="511ae-145">String</span><span class="sxs-lookup"><span data-stu-id="511ae-145">String</span></span> | <span data-ttu-id="511ae-146">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="511ae-146">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="511ae-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="511ae-147">highestGrade</span></span>|<span data-ttu-id="511ae-148">String</span><span class="sxs-lookup"><span data-stu-id="511ae-148">String</span></span>| <span data-ttu-id="511ae-149">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="511ae-149">Highest grade taught.</span></span> |
|<span data-ttu-id="511ae-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="511ae-150">lowestGrade</span></span>|<span data-ttu-id="511ae-151">String</span><span class="sxs-lookup"><span data-stu-id="511ae-151">String</span></span>| <span data-ttu-id="511ae-152">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="511ae-152">Lowest grade taught.</span></span> |
|<span data-ttu-id="511ae-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="511ae-153">schoolNumber</span></span>|<span data-ttu-id="511ae-154">String</span><span class="sxs-lookup"><span data-stu-id="511ae-154">String</span></span>| <span data-ttu-id="511ae-155">学校番号。</span><span class="sxs-lookup"><span data-stu-id="511ae-155">School Number.</span></span>|
|<span data-ttu-id="511ae-156">externalId</span><span class="sxs-lookup"><span data-stu-id="511ae-156">externalId</span></span>|<span data-ttu-id="511ae-157">String</span><span class="sxs-lookup"><span data-stu-id="511ae-157">String</span></span>| <span data-ttu-id="511ae-158">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="511ae-158">Id of school in syncing system.</span></span> |
|<span data-ttu-id="511ae-159">phone</span><span class="sxs-lookup"><span data-stu-id="511ae-159">phone</span></span>|<span data-ttu-id="511ae-160">String</span><span class="sxs-lookup"><span data-stu-id="511ae-160">String</span></span>| <span data-ttu-id="511ae-161">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="511ae-161">Phone number of school.</span></span> |
|<span data-ttu-id="511ae-162">fax</span><span class="sxs-lookup"><span data-stu-id="511ae-162">fax</span></span>|<span data-ttu-id="511ae-163">String</span><span class="sxs-lookup"><span data-stu-id="511ae-163">String</span></span>| <span data-ttu-id="511ae-164">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="511ae-164">Fax number of school.</span></span> |
|<span data-ttu-id="511ae-165">address</span><span class="sxs-lookup"><span data-stu-id="511ae-165">address</span></span>|[<span data-ttu-id="511ae-166">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="511ae-166">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="511ae-167">学校のアドレス。</span><span class="sxs-lookup"><span data-stu-id="511ae-167">Address of the School.</span></span>|
|<span data-ttu-id="511ae-168">createdBy</span><span class="sxs-lookup"><span data-stu-id="511ae-168">createdBy</span></span>|[<span data-ttu-id="511ae-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="511ae-169">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="511ae-170">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="511ae-170">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="511ae-171">応答</span><span class="sxs-lookup"><span data-stu-id="511ae-171">Response</span></span>
<span data-ttu-id="511ae-172">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="511ae-172">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="511ae-173">例</span><span class="sxs-lookup"><span data-stu-id="511ae-173">Example</span></span>
##### <a name="request"></a><span data-ttu-id="511ae-174">要求</span><span class="sxs-lookup"><span data-stu-id="511ae-174">Request</span></span>
<span data-ttu-id="511ae-175">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="511ae-175">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="511ae-176">応答</span><span class="sxs-lookup"><span data-stu-id="511ae-176">Response</span></span>
<span data-ttu-id="511ae-177">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="511ae-177">The following is an example of the response.</span></span> 

><span data-ttu-id="511ae-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="511ae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
