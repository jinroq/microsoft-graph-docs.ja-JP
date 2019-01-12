---
title: Orgcontact を更新します。
description: Orgcontact オブジェクトのプロパティを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f7943234dbff62da070b51a3ae6d92d2bdb28d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938819"
---
# <a name="update-orgcontact"></a><span data-ttu-id="0976f-103">Orgcontact を更新します。</span><span class="sxs-lookup"><span data-stu-id="0976f-103">Update orgcontact</span></span>

> <span data-ttu-id="0976f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0976f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0976f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0976f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0976f-106">Orgcontact オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0976f-106">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0976f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0976f-107">Permissions</span></span>
<span data-ttu-id="0976f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0976f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0976f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0976f-110">Permission type</span></span>      | <span data-ttu-id="0976f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0976f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0976f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0976f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0976f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0976f-113">Not supported.</span></span>    |
|<span data-ttu-id="0976f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0976f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0976f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0976f-115">Not supported.</span></span>    |
|<span data-ttu-id="0976f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0976f-116">Application</span></span> | <span data-ttu-id="0976f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0976f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0976f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0976f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0976f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0976f-119">Request headers</span></span>
| <span data-ttu-id="0976f-120">名前</span><span class="sxs-lookup"><span data-stu-id="0976f-120">Name</span></span>       | <span data-ttu-id="0976f-121">型</span><span class="sxs-lookup"><span data-stu-id="0976f-121">Type</span></span> | <span data-ttu-id="0976f-122">説明</span><span class="sxs-lookup"><span data-stu-id="0976f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0976f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0976f-123">Authorization</span></span>  | <span data-ttu-id="0976f-124">string</span><span class="sxs-lookup"><span data-stu-id="0976f-124">string</span></span>  | <span data-ttu-id="0976f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0976f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0976f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0976f-127">Request body</span></span>
<span data-ttu-id="0976f-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0976f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0976f-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0976f-131">Property</span></span>     | <span data-ttu-id="0976f-132">型</span><span class="sxs-lookup"><span data-stu-id="0976f-132">Type</span></span>   |<span data-ttu-id="0976f-133">説明</span><span class="sxs-lookup"><span data-stu-id="0976f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0976f-134">city</span><span class="sxs-lookup"><span data-stu-id="0976f-134">city</span></span>|<span data-ttu-id="0976f-135">String</span><span class="sxs-lookup"><span data-stu-id="0976f-135">String</span></span>||
|<span data-ttu-id="0976f-136">country</span><span class="sxs-lookup"><span data-stu-id="0976f-136">country</span></span>|<span data-ttu-id="0976f-137">String</span><span class="sxs-lookup"><span data-stu-id="0976f-137">String</span></span>||
|<span data-ttu-id="0976f-138">department</span><span class="sxs-lookup"><span data-stu-id="0976f-138">department</span></span>|<span data-ttu-id="0976f-139">String</span><span class="sxs-lookup"><span data-stu-id="0976f-139">String</span></span>||
|<span data-ttu-id="0976f-140">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="0976f-140">onPremisesSyncEnabled</span></span>|<span data-ttu-id="0976f-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0976f-141">Boolean</span></span>||
|<span data-ttu-id="0976f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0976f-142">displayName</span></span>|<span data-ttu-id="0976f-143">String</span><span class="sxs-lookup"><span data-stu-id="0976f-143">String</span></span>||
|<span data-ttu-id="0976f-144">givenName</span><span class="sxs-lookup"><span data-stu-id="0976f-144">givenName</span></span>|<span data-ttu-id="0976f-145">String</span><span class="sxs-lookup"><span data-stu-id="0976f-145">String</span></span>||
|<span data-ttu-id="0976f-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0976f-146">jobTitle</span></span>|<span data-ttu-id="0976f-147">String</span><span class="sxs-lookup"><span data-stu-id="0976f-147">String</span></span>||
|<span data-ttu-id="0976f-148">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0976f-148">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="0976f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0976f-149">DateTimeOffset</span></span>||
|<span data-ttu-id="0976f-150">mail</span><span class="sxs-lookup"><span data-stu-id="0976f-150">mail</span></span>|<span data-ttu-id="0976f-151">String</span><span class="sxs-lookup"><span data-stu-id="0976f-151">String</span></span>||
|<span data-ttu-id="0976f-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0976f-152">mailNickname</span></span>|<span data-ttu-id="0976f-153">String</span><span class="sxs-lookup"><span data-stu-id="0976f-153">String</span></span>||
|<span data-ttu-id="0976f-154">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0976f-154">mobilePhone</span></span>|<span data-ttu-id="0976f-155">String</span><span class="sxs-lookup"><span data-stu-id="0976f-155">String</span></span>||
|<span data-ttu-id="0976f-156">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0976f-156">officeLocation</span></span>|<span data-ttu-id="0976f-157">String</span><span class="sxs-lookup"><span data-stu-id="0976f-157">String</span></span>||
|<span data-ttu-id="0976f-158">postalCode</span><span class="sxs-lookup"><span data-stu-id="0976f-158">postalCode</span></span>|<span data-ttu-id="0976f-159">String</span><span class="sxs-lookup"><span data-stu-id="0976f-159">String</span></span>||
|<span data-ttu-id="0976f-160">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="0976f-160">proxyAddresses</span></span>|<span data-ttu-id="0976f-161">String</span><span class="sxs-lookup"><span data-stu-id="0976f-161">String</span></span>||
|<span data-ttu-id="0976f-162">state</span><span class="sxs-lookup"><span data-stu-id="0976f-162">state</span></span>|<span data-ttu-id="0976f-163">String</span><span class="sxs-lookup"><span data-stu-id="0976f-163">String</span></span>||
|<span data-ttu-id="0976f-164">streetAddress</span><span class="sxs-lookup"><span data-stu-id="0976f-164">streetAddress</span></span>|<span data-ttu-id="0976f-165">String</span><span class="sxs-lookup"><span data-stu-id="0976f-165">String</span></span>||
|<span data-ttu-id="0976f-166">surname</span><span class="sxs-lookup"><span data-stu-id="0976f-166">surname</span></span>|<span data-ttu-id="0976f-167">String</span><span class="sxs-lookup"><span data-stu-id="0976f-167">String</span></span>||
|<span data-ttu-id="0976f-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="0976f-168">businessPhones</span></span>|<span data-ttu-id="0976f-169">String</span><span class="sxs-lookup"><span data-stu-id="0976f-169">String</span></span>||

## <a name="response"></a><span data-ttu-id="0976f-170">応答</span><span class="sxs-lookup"><span data-stu-id="0976f-170">Response</span></span>

<span data-ttu-id="0976f-171">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の更新された[orgContact](../resources/orgcontact.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0976f-171">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0976f-172">例</span><span class="sxs-lookup"><span data-stu-id="0976f-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0976f-173">要求</span><span class="sxs-lookup"><span data-stu-id="0976f-173">Request</span></span>
<span data-ttu-id="0976f-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0976f-174">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0976f-175">応答</span><span class="sxs-lookup"><span data-stu-id="0976f-175">Response</span></span>
<span data-ttu-id="0976f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0976f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
