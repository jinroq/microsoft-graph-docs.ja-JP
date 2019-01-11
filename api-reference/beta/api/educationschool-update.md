---
title: educationschool プロパティを更新する
description: 学校オブジェクトのプロパティを更新します。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 23c7c476e2447fbde43a0e7521d4b3d626f80f5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892233"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="fd5ea-103">educationschool プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="fd5ea-103">Update educationschool properties</span></span>

> <span data-ttu-id="fd5ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd5ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd5ea-106">学校オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-106">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd5ea-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd5ea-107">Permissions</span></span>
<span data-ttu-id="fd5ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd5ea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd5ea-110">Permission type</span></span>      | <span data-ttu-id="fd5ea-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd5ea-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd5ea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd5ea-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="fd5ea-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-113">Not supported.</span></span>  |
|<span data-ttu-id="fd5ea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd5ea-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fd5ea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-115">Not supported.</span></span>  |
|<span data-ttu-id="fd5ea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd5ea-116">Application</span></span> | <span data-ttu-id="fd5ea-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd5ea-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd5ea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd5ea-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fd5ea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd5ea-119">Request headers</span></span>
| <span data-ttu-id="fd5ea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd5ea-120">Header</span></span>       | <span data-ttu-id="fd5ea-121">値</span><span class="sxs-lookup"><span data-stu-id="fd5ea-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd5ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd5ea-122">Authorization</span></span>  | <span data-ttu-id="fd5ea-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd5ea-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd5ea-125">Content-Type</span></span>  | <span data-ttu-id="fd5ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd5ea-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd5ea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd5ea-127">Request body</span></span>
<span data-ttu-id="fd5ea-128">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="fd5ea-129">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fd5ea-130">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd5ea-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd5ea-131">Property</span></span>     | <span data-ttu-id="fd5ea-132">種類</span><span class="sxs-lookup"><span data-stu-id="fd5ea-132">Type</span></span>   |<span data-ttu-id="fd5ea-133">説明</span><span class="sxs-lookup"><span data-stu-id="fd5ea-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd5ea-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fd5ea-134">displayName</span></span>| <span data-ttu-id="fd5ea-135">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-135">String</span></span>| <span data-ttu-id="fd5ea-136">学校の表示名</span><span class="sxs-lookup"><span data-stu-id="fd5ea-136">Display name of the school</span></span>| 
|<span data-ttu-id="fd5ea-137">説明</span><span class="sxs-lookup"><span data-stu-id="fd5ea-137">description</span></span>| <span data-ttu-id="fd5ea-138">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-138">String</span></span> | <span data-ttu-id="fd5ea-139">学校の説明</span><span class="sxs-lookup"><span data-stu-id="fd5ea-139">Description of the school</span></span>| 
|<span data-ttu-id="fd5ea-140">principalEmail</span><span class="sxs-lookup"><span data-stu-id="fd5ea-140">principalEmail</span></span>| <span data-ttu-id="fd5ea-141">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-141">String</span></span>| <span data-ttu-id="fd5ea-142">プリンシパルの電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="fd5ea-142">Email address of the principal</span></span>|
|<span data-ttu-id="fd5ea-143">principalName</span><span class="sxs-lookup"><span data-stu-id="fd5ea-143">principalName</span></span>| <span data-ttu-id="fd5ea-144">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-144">String</span></span> | <span data-ttu-id="fd5ea-145">プリンシパルの名前</span><span class="sxs-lookup"><span data-stu-id="fd5ea-145">Name of the principal</span></span>|
|<span data-ttu-id="fd5ea-146">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="fd5ea-146">externalPrincipalId</span></span>| <span data-ttu-id="fd5ea-147">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-147">String</span></span> | <span data-ttu-id="fd5ea-148">同期システム内のプリンシパルの ID。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-148">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="fd5ea-149">highestGrade</span><span class="sxs-lookup"><span data-stu-id="fd5ea-149">highestGrade</span></span>|<span data-ttu-id="fd5ea-150">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-150">String</span></span>| <span data-ttu-id="fd5ea-151">授業を受けている最高学年。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-151">Highest grade taught.</span></span> |
|<span data-ttu-id="fd5ea-152">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="fd5ea-152">lowestGrade</span></span>|<span data-ttu-id="fd5ea-153">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-153">String</span></span>| <span data-ttu-id="fd5ea-154">授業を受けている最低学年。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-154">Lowest grade taught.</span></span> |
|<span data-ttu-id="fd5ea-155">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="fd5ea-155">schoolNumber</span></span>|<span data-ttu-id="fd5ea-156">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-156">String</span></span>| <span data-ttu-id="fd5ea-157">学校番号。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-157">School Number.</span></span>|
|<span data-ttu-id="fd5ea-158">externalId</span><span class="sxs-lookup"><span data-stu-id="fd5ea-158">externalId</span></span>|<span data-ttu-id="fd5ea-159">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-159">String</span></span>| <span data-ttu-id="fd5ea-160">同期システム内の学校の ID。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-160">Id of school in syncing system.</span></span> |
|<span data-ttu-id="fd5ea-161">phone</span><span class="sxs-lookup"><span data-stu-id="fd5ea-161">phone</span></span>|<span data-ttu-id="fd5ea-162">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-162">String</span></span>| <span data-ttu-id="fd5ea-163">学校の電話番号。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-163">Phone number of school.</span></span> |
|<span data-ttu-id="fd5ea-164">fax</span><span class="sxs-lookup"><span data-stu-id="fd5ea-164">fax</span></span>|<span data-ttu-id="fd5ea-165">String</span><span class="sxs-lookup"><span data-stu-id="fd5ea-165">String</span></span>| <span data-ttu-id="fd5ea-166">学校の FAX 番号。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-166">Fax number of school.</span></span> |
|<span data-ttu-id="fd5ea-167">address</span><span class="sxs-lookup"><span data-stu-id="fd5ea-167">address</span></span>|[<span data-ttu-id="fd5ea-168">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="fd5ea-168">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="fd5ea-169">学校のアドレス。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-169">Address of the School.</span></span>|
|<span data-ttu-id="fd5ea-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="fd5ea-170">createdBy</span></span>|[<span data-ttu-id="fd5ea-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="fd5ea-171">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="fd5ea-172">学校を作成したエンティティ。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-172">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="fd5ea-173">応答</span><span class="sxs-lookup"><span data-stu-id="fd5ea-173">Response</span></span>
<span data-ttu-id="fd5ea-174">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [educationSchool](../resources/educationschool.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-174">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd5ea-175">例</span><span class="sxs-lookup"><span data-stu-id="fd5ea-175">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd5ea-176">要求</span><span class="sxs-lookup"><span data-stu-id="fd5ea-176">Request</span></span>
<span data-ttu-id="fd5ea-177">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-177">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="fd5ea-178">応答</span><span class="sxs-lookup"><span data-stu-id="fd5ea-178">Response</span></span>
<span data-ttu-id="fd5ea-179">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-179">The following is an example of the response.</span></span> 

><span data-ttu-id="fd5ea-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fd5ea-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
