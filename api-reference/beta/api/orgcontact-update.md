---
title: orgcontact への更新
description: orgcontact へオブジェクトのプロパティを更新します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cec4817472fe5192c7af836131cea83bcb60d77b
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789635"
---
# <a name="update-orgcontact"></a><span data-ttu-id="80600-103">orgcontact への更新</span><span class="sxs-lookup"><span data-stu-id="80600-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80600-104">orgcontact へオブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="80600-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="80600-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80600-105">Permissions</span></span>
<span data-ttu-id="80600-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80600-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80600-108">Permission type</span></span>      | <span data-ttu-id="80600-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80600-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80600-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80600-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80600-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80600-111">Not supported.</span></span>    |
|<span data-ttu-id="80600-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80600-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80600-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80600-113">Not supported.</span></span>    |
|<span data-ttu-id="80600-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80600-114">Application</span></span> | <span data-ttu-id="80600-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80600-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80600-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80600-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="80600-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80600-117">Request headers</span></span>
| <span data-ttu-id="80600-118">名前</span><span class="sxs-lookup"><span data-stu-id="80600-118">Name</span></span>       | <span data-ttu-id="80600-119">種類</span><span class="sxs-lookup"><span data-stu-id="80600-119">Type</span></span> | <span data-ttu-id="80600-120">説明</span><span class="sxs-lookup"><span data-stu-id="80600-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80600-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80600-121">Authorization</span></span>  | <span data-ttu-id="80600-122">string</span><span class="sxs-lookup"><span data-stu-id="80600-122">string</span></span>  | <span data-ttu-id="80600-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="80600-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80600-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="80600-125">Request body</span></span>
<span data-ttu-id="80600-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="80600-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80600-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80600-129">Property</span></span>     | <span data-ttu-id="80600-130">種類</span><span class="sxs-lookup"><span data-stu-id="80600-130">Type</span></span>   |<span data-ttu-id="80600-131">説明</span><span class="sxs-lookup"><span data-stu-id="80600-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80600-132">city</span><span class="sxs-lookup"><span data-stu-id="80600-132">city</span></span>|<span data-ttu-id="80600-133">String</span><span class="sxs-lookup"><span data-stu-id="80600-133">String</span></span>||
|<span data-ttu-id="80600-134">country</span><span class="sxs-lookup"><span data-stu-id="80600-134">country</span></span>|<span data-ttu-id="80600-135">String</span><span class="sxs-lookup"><span data-stu-id="80600-135">String</span></span>||
|<span data-ttu-id="80600-136">department</span><span class="sxs-lookup"><span data-stu-id="80600-136">department</span></span>|<span data-ttu-id="80600-137">String</span><span class="sxs-lookup"><span data-stu-id="80600-137">String</span></span>||
|<span data-ttu-id="80600-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="80600-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="80600-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="80600-139">Boolean</span></span>||
|<span data-ttu-id="80600-140">displayName</span><span class="sxs-lookup"><span data-stu-id="80600-140">displayName</span></span>|<span data-ttu-id="80600-141">String</span><span class="sxs-lookup"><span data-stu-id="80600-141">String</span></span>||
|<span data-ttu-id="80600-142">givenName</span><span class="sxs-lookup"><span data-stu-id="80600-142">givenName</span></span>|<span data-ttu-id="80600-143">String</span><span class="sxs-lookup"><span data-stu-id="80600-143">String</span></span>||
|<span data-ttu-id="80600-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="80600-144">jobTitle</span></span>|<span data-ttu-id="80600-145">String</span><span class="sxs-lookup"><span data-stu-id="80600-145">String</span></span>||
|<span data-ttu-id="80600-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80600-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="80600-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80600-147">DateTimeOffset</span></span>||
|<span data-ttu-id="80600-148">mail</span><span class="sxs-lookup"><span data-stu-id="80600-148">mail</span></span>|<span data-ttu-id="80600-149">String</span><span class="sxs-lookup"><span data-stu-id="80600-149">String</span></span>||
|<span data-ttu-id="80600-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="80600-150">mailNickname</span></span>|<span data-ttu-id="80600-151">String</span><span class="sxs-lookup"><span data-stu-id="80600-151">String</span></span>||
|<span data-ttu-id="80600-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="80600-152">mobilePhone</span></span>|<span data-ttu-id="80600-153">String</span><span class="sxs-lookup"><span data-stu-id="80600-153">String</span></span>||
|<span data-ttu-id="80600-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="80600-154">officeLocation</span></span>|<span data-ttu-id="80600-155">String</span><span class="sxs-lookup"><span data-stu-id="80600-155">String</span></span>||
|<span data-ttu-id="80600-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="80600-156">postalCode</span></span>|<span data-ttu-id="80600-157">String</span><span class="sxs-lookup"><span data-stu-id="80600-157">String</span></span>||
|<span data-ttu-id="80600-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="80600-158">proxyAddresses</span></span>|<span data-ttu-id="80600-159">String</span><span class="sxs-lookup"><span data-stu-id="80600-159">String</span></span>||
|<span data-ttu-id="80600-160">state</span><span class="sxs-lookup"><span data-stu-id="80600-160">state</span></span>|<span data-ttu-id="80600-161">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="80600-161">String</span></span>||
|<span data-ttu-id="80600-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="80600-162">streetAddress</span></span>|<span data-ttu-id="80600-163">String</span><span class="sxs-lookup"><span data-stu-id="80600-163">String</span></span>||
|<span data-ttu-id="80600-164">surname</span><span class="sxs-lookup"><span data-stu-id="80600-164">surname</span></span>|<span data-ttu-id="80600-165">String</span><span class="sxs-lookup"><span data-stu-id="80600-165">String</span></span>||
|<span data-ttu-id="80600-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="80600-166">businessPhones</span></span>|<span data-ttu-id="80600-167">String collection</span><span class="sxs-lookup"><span data-stu-id="80600-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="80600-168">応答</span><span class="sxs-lookup"><span data-stu-id="80600-168">Response</span></span>

<span data-ttu-id="80600-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[orgcontact](../resources/orgcontact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80600-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80600-170">例</span><span class="sxs-lookup"><span data-stu-id="80600-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80600-171">要求</span><span class="sxs-lookup"><span data-stu-id="80600-171">Request</span></span>
<span data-ttu-id="80600-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80600-172">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="80600-173">応答</span><span class="sxs-lookup"><span data-stu-id="80600-173">Response</span></span>
<span data-ttu-id="80600-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80600-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
