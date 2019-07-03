---
title: Orgcontact への更新
description: Orgcontact へオブジェクトのプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d044d1d0add2887a690fa6e6b5ac3d00d9e9757
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450633"
---
# <a name="update-orgcontact"></a><span data-ttu-id="40c47-103">Orgcontact への更新</span><span class="sxs-lookup"><span data-stu-id="40c47-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40c47-104">Orgcontact へオブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="40c47-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40c47-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="40c47-105">Permissions</span></span>
<span data-ttu-id="40c47-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40c47-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40c47-108">Permission type</span></span>      | <span data-ttu-id="40c47-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="40c47-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40c47-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40c47-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40c47-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40c47-111">Not supported.</span></span>    |
|<span data-ttu-id="40c47-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40c47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40c47-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40c47-113">Not supported.</span></span>    |
|<span data-ttu-id="40c47-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40c47-114">Application</span></span> | <span data-ttu-id="40c47-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40c47-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40c47-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40c47-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40c47-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40c47-117">Request headers</span></span>
| <span data-ttu-id="40c47-118">名前</span><span class="sxs-lookup"><span data-stu-id="40c47-118">Name</span></span>       | <span data-ttu-id="40c47-119">型</span><span class="sxs-lookup"><span data-stu-id="40c47-119">Type</span></span> | <span data-ttu-id="40c47-120">説明</span><span class="sxs-lookup"><span data-stu-id="40c47-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40c47-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40c47-121">Authorization</span></span>  | <span data-ttu-id="40c47-122">string</span><span class="sxs-lookup"><span data-stu-id="40c47-122">string</span></span>  | <span data-ttu-id="40c47-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="40c47-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40c47-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="40c47-125">Request body</span></span>
<span data-ttu-id="40c47-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="40c47-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40c47-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="40c47-129">Property</span></span>     | <span data-ttu-id="40c47-130">型</span><span class="sxs-lookup"><span data-stu-id="40c47-130">Type</span></span>   |<span data-ttu-id="40c47-131">説明</span><span class="sxs-lookup"><span data-stu-id="40c47-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40c47-132">city</span><span class="sxs-lookup"><span data-stu-id="40c47-132">city</span></span>|<span data-ttu-id="40c47-133">String</span><span class="sxs-lookup"><span data-stu-id="40c47-133">String</span></span>||
|<span data-ttu-id="40c47-134">country</span><span class="sxs-lookup"><span data-stu-id="40c47-134">country</span></span>|<span data-ttu-id="40c47-135">String</span><span class="sxs-lookup"><span data-stu-id="40c47-135">String</span></span>||
|<span data-ttu-id="40c47-136">department</span><span class="sxs-lookup"><span data-stu-id="40c47-136">department</span></span>|<span data-ttu-id="40c47-137">String</span><span class="sxs-lookup"><span data-stu-id="40c47-137">String</span></span>||
|<span data-ttu-id="40c47-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="40c47-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="40c47-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="40c47-139">Boolean</span></span>||
|<span data-ttu-id="40c47-140">displayName</span><span class="sxs-lookup"><span data-stu-id="40c47-140">displayName</span></span>|<span data-ttu-id="40c47-141">文字列</span><span class="sxs-lookup"><span data-stu-id="40c47-141">String</span></span>||
|<span data-ttu-id="40c47-142">givenName</span><span class="sxs-lookup"><span data-stu-id="40c47-142">givenName</span></span>|<span data-ttu-id="40c47-143">String</span><span class="sxs-lookup"><span data-stu-id="40c47-143">String</span></span>||
|<span data-ttu-id="40c47-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="40c47-144">jobTitle</span></span>|<span data-ttu-id="40c47-145">String</span><span class="sxs-lookup"><span data-stu-id="40c47-145">String</span></span>||
|<span data-ttu-id="40c47-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="40c47-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="40c47-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40c47-147">DateTimeOffset</span></span>||
|<span data-ttu-id="40c47-148">mail</span><span class="sxs-lookup"><span data-stu-id="40c47-148">mail</span></span>|<span data-ttu-id="40c47-149">String</span><span class="sxs-lookup"><span data-stu-id="40c47-149">String</span></span>||
|<span data-ttu-id="40c47-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="40c47-150">mailNickname</span></span>|<span data-ttu-id="40c47-151">String</span><span class="sxs-lookup"><span data-stu-id="40c47-151">String</span></span>||
|<span data-ttu-id="40c47-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="40c47-152">mobilePhone</span></span>|<span data-ttu-id="40c47-153">String</span><span class="sxs-lookup"><span data-stu-id="40c47-153">String</span></span>||
|<span data-ttu-id="40c47-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="40c47-154">officeLocation</span></span>|<span data-ttu-id="40c47-155">String</span><span class="sxs-lookup"><span data-stu-id="40c47-155">String</span></span>||
|<span data-ttu-id="40c47-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="40c47-156">postalCode</span></span>|<span data-ttu-id="40c47-157">String</span><span class="sxs-lookup"><span data-stu-id="40c47-157">String</span></span>||
|<span data-ttu-id="40c47-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="40c47-158">proxyAddresses</span></span>|<span data-ttu-id="40c47-159">String</span><span class="sxs-lookup"><span data-stu-id="40c47-159">String</span></span>||
|<span data-ttu-id="40c47-160">state</span><span class="sxs-lookup"><span data-stu-id="40c47-160">state</span></span>|<span data-ttu-id="40c47-161">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="40c47-161">String</span></span>||
|<span data-ttu-id="40c47-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="40c47-162">streetAddress</span></span>|<span data-ttu-id="40c47-163">String</span><span class="sxs-lookup"><span data-stu-id="40c47-163">String</span></span>||
|<span data-ttu-id="40c47-164">surname</span><span class="sxs-lookup"><span data-stu-id="40c47-164">surname</span></span>|<span data-ttu-id="40c47-165">String</span><span class="sxs-lookup"><span data-stu-id="40c47-165">String</span></span>||
|<span data-ttu-id="40c47-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="40c47-166">businessPhones</span></span>|<span data-ttu-id="40c47-167">String collection</span><span class="sxs-lookup"><span data-stu-id="40c47-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="40c47-168">応答</span><span class="sxs-lookup"><span data-stu-id="40c47-168">Response</span></span>

<span data-ttu-id="40c47-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[orgcontact](../resources/orgcontact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="40c47-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40c47-170">例</span><span class="sxs-lookup"><span data-stu-id="40c47-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40c47-171">要求</span><span class="sxs-lookup"><span data-stu-id="40c47-171">Request</span></span>
<span data-ttu-id="40c47-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40c47-172">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40c47-173">プロトコル</span><span class="sxs-lookup"><span data-stu-id="40c47-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40c47-174">C#</span><span class="sxs-lookup"><span data-stu-id="40c47-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40c47-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="40c47-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40c47-176">目的-C</span><span class="sxs-lookup"><span data-stu-id="40c47-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="40c47-177">応答</span><span class="sxs-lookup"><span data-stu-id="40c47-177">Response</span></span>
<span data-ttu-id="40c47-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40c47-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
