---
title: Orgcontact を更新します。
description: Orgcontact オブジェクトのプロパティを更新します。
ms.openlocfilehash: 04bc5bef07fb49c2c4fe730e89517de2f364628a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068702"
---
# <a name="update-orgcontact"></a><span data-ttu-id="34d94-103">Orgcontact を更新します。</span><span class="sxs-lookup"><span data-stu-id="34d94-103">Update orgcontact</span></span>

> <span data-ttu-id="34d94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34d94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34d94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34d94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34d94-106">Orgcontact オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="34d94-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="34d94-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34d94-107">Permissions</span></span>
<span data-ttu-id="34d94-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34d94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34d94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34d94-110">Permission type</span></span>      | <span data-ttu-id="34d94-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34d94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34d94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34d94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34d94-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34d94-113">Not supported.</span></span>    |
|<span data-ttu-id="34d94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34d94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34d94-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34d94-115">Not supported.</span></span>    |
|<span data-ttu-id="34d94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34d94-116">Application</span></span> | <span data-ttu-id="34d94-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34d94-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34d94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34d94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="34d94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34d94-119">Request headers</span></span>
| <span data-ttu-id="34d94-120">名前</span><span class="sxs-lookup"><span data-stu-id="34d94-120">Name</span></span>       | <span data-ttu-id="34d94-121">型</span><span class="sxs-lookup"><span data-stu-id="34d94-121">Type</span></span> | <span data-ttu-id="34d94-122">説明</span><span class="sxs-lookup"><span data-stu-id="34d94-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34d94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34d94-123">Authorization</span></span>  | <span data-ttu-id="34d94-124">string</span><span class="sxs-lookup"><span data-stu-id="34d94-124">string</span></span>  | <span data-ttu-id="34d94-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34d94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34d94-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="34d94-127">Request body</span></span>
<span data-ttu-id="34d94-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="34d94-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="34d94-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34d94-131">Property</span></span>     | <span data-ttu-id="34d94-132">型</span><span class="sxs-lookup"><span data-stu-id="34d94-132">Type</span></span>   |<span data-ttu-id="34d94-133">説明</span><span class="sxs-lookup"><span data-stu-id="34d94-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34d94-134">city</span><span class="sxs-lookup"><span data-stu-id="34d94-134">city</span></span>|<span data-ttu-id="34d94-135">String</span><span class="sxs-lookup"><span data-stu-id="34d94-135">String</span></span>||
|<span data-ttu-id="34d94-136">country</span><span class="sxs-lookup"><span data-stu-id="34d94-136">country</span></span>|<span data-ttu-id="34d94-137">String</span><span class="sxs-lookup"><span data-stu-id="34d94-137">String</span></span>||
|<span data-ttu-id="34d94-138">department</span><span class="sxs-lookup"><span data-stu-id="34d94-138">department</span></span>|<span data-ttu-id="34d94-139">String</span><span class="sxs-lookup"><span data-stu-id="34d94-139">String</span></span>||
|<span data-ttu-id="34d94-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="34d94-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="34d94-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="34d94-141">Boolean</span></span>||
|<span data-ttu-id="34d94-142">displayName</span><span class="sxs-lookup"><span data-stu-id="34d94-142">displayName</span></span>|<span data-ttu-id="34d94-143">String</span><span class="sxs-lookup"><span data-stu-id="34d94-143">String</span></span>||
|<span data-ttu-id="34d94-144">givenName</span><span class="sxs-lookup"><span data-stu-id="34d94-144">givenName</span></span>|<span data-ttu-id="34d94-145">String</span><span class="sxs-lookup"><span data-stu-id="34d94-145">String</span></span>||
|<span data-ttu-id="34d94-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="34d94-146">jobTitle</span></span>|<span data-ttu-id="34d94-147">String</span><span class="sxs-lookup"><span data-stu-id="34d94-147">String</span></span>||
|<span data-ttu-id="34d94-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="34d94-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="34d94-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34d94-149">DateTimeOffset</span></span>||
|<span data-ttu-id="34d94-150">mail</span><span class="sxs-lookup"><span data-stu-id="34d94-150">mail</span></span>|<span data-ttu-id="34d94-151">String</span><span class="sxs-lookup"><span data-stu-id="34d94-151">String</span></span>||
|<span data-ttu-id="34d94-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="34d94-152">mailNickname</span></span>|<span data-ttu-id="34d94-153">String</span><span class="sxs-lookup"><span data-stu-id="34d94-153">String</span></span>||
|<span data-ttu-id="34d94-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="34d94-154">mobilePhone</span></span>|<span data-ttu-id="34d94-155">String</span><span class="sxs-lookup"><span data-stu-id="34d94-155">String</span></span>||
|<span data-ttu-id="34d94-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="34d94-156">officeLocation</span></span>|<span data-ttu-id="34d94-157">String</span><span class="sxs-lookup"><span data-stu-id="34d94-157">String</span></span>||
|<span data-ttu-id="34d94-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="34d94-158">postalCode</span></span>|<span data-ttu-id="34d94-159">String</span><span class="sxs-lookup"><span data-stu-id="34d94-159">String</span></span>||
|<span data-ttu-id="34d94-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="34d94-160">proxyAddresses</span></span>|<span data-ttu-id="34d94-161">String</span><span class="sxs-lookup"><span data-stu-id="34d94-161">String</span></span>||
|<span data-ttu-id="34d94-162">state</span><span class="sxs-lookup"><span data-stu-id="34d94-162">state</span></span>|<span data-ttu-id="34d94-163">String</span><span class="sxs-lookup"><span data-stu-id="34d94-163">String</span></span>||
|<span data-ttu-id="34d94-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="34d94-164">streetAddress</span></span>|<span data-ttu-id="34d94-165">String</span><span class="sxs-lookup"><span data-stu-id="34d94-165">String</span></span>||
|<span data-ttu-id="34d94-166">surname</span><span class="sxs-lookup"><span data-stu-id="34d94-166">surname</span></span>|<span data-ttu-id="34d94-167">String</span><span class="sxs-lookup"><span data-stu-id="34d94-167">String</span></span>||
|<span data-ttu-id="34d94-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="34d94-168">businessPhones</span></span>|<span data-ttu-id="34d94-169">String</span><span class="sxs-lookup"><span data-stu-id="34d94-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="34d94-170">応答</span><span class="sxs-lookup"><span data-stu-id="34d94-170">Response</span></span>

<span data-ttu-id="34d94-171">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[orgContact](../resources/orgcontact.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="34d94-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34d94-172">例</span><span class="sxs-lookup"><span data-stu-id="34d94-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34d94-173">要求</span><span class="sxs-lookup"><span data-stu-id="34d94-173">Request</span></span>
<span data-ttu-id="34d94-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34d94-174">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="34d94-175">応答</span><span class="sxs-lookup"><span data-stu-id="34d94-175">Response</span></span>
<span data-ttu-id="34d94-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34d94-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->