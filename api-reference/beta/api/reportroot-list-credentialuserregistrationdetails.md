---
title: CredentialUserRegistrationDetails を一覧表示する
description: 指定したテナントの credentialUserRegistrationDetails オブジェクトの一覧を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: bbb4c1b71e596eebc4055732b0423c2b0fd55786
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871204"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="6bef9-103">CredentialUserRegistrationDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6bef9-103">List credentialUserRegistrationDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bef9-104">指定したテナントの[Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-104">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bef9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6bef9-105">Permissions</span></span>

<span data-ttu-id="6bef9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6bef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6bef9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6bef9-108">Permission type</span></span>                        | <span data-ttu-id="6bef9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6bef9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6bef9-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="6bef9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bef9-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bef9-111">Reports.Read.All</span></span> |
| <span data-ttu-id="6bef9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6bef9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bef9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bef9-113">Not supported.</span></span> |
| <span data-ttu-id="6bef9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6bef9-114">Application</span></span>                            | <span data-ttu-id="6bef9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bef9-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bef9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6bef9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6bef9-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6bef9-117">Optional query parameters</span></span>

<span data-ttu-id="6bef9-118">この関数は、オプションの OData クエリパラメーター **$filter**をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6bef9-118">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="6bef9-119">**$Filter**は、 [Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)リソースの次のプロパティの1つ以上に適用できます。</span><span class="sxs-lookup"><span data-stu-id="6bef9-119">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="6bef9-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bef9-120">Properties</span></span> | <span data-ttu-id="6bef9-121">説明と例</span><span class="sxs-lookup"><span data-stu-id="6bef9-121">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="6bef9-122">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6bef9-122">userDisplayName</span></span> | <span data-ttu-id="6bef9-123">ユーザー名でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-123">Filter by user name.</span></span> <span data-ttu-id="6bef9-124">例: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-124">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="6bef9-125">サポートされて`eq`いるフィルター `startswith()`演算子:、、。</span><span class="sxs-lookup"><span data-stu-id="6bef9-125">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="6bef9-126">大文字小文字の区別をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6bef9-126">Supports case insensitive.</span></span> |
| <span data-ttu-id="6bef9-127">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6bef9-127">userPrincipalName</span></span> | <span data-ttu-id="6bef9-128">ユーザープリンシパル名でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-128">Filter by user principal name.</span></span> <span data-ttu-id="6bef9-129">例: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-129">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="6bef9-130">サポートされて`eq`いる`startswith()`フィルター演算子: および。</span><span class="sxs-lookup"><span data-stu-id="6bef9-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="6bef9-131">大文字小文字の区別をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6bef9-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="6bef9-132">authMethods</span><span class="sxs-lookup"><span data-stu-id="6bef9-132">authMethods</span></span> | <span data-ttu-id="6bef9-133">登録時に使用される認証方法でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-133">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="6bef9-134">例: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-134">For example: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="6bef9-135">サポートされて`eq`いるフィルター演算子:。</span><span class="sxs-lookup"><span data-stu-id="6bef9-135">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="6bef9-136">isRegistered</span><span class="sxs-lookup"><span data-stu-id="6bef9-136">isRegistered</span></span> | <span data-ttu-id="6bef9-137">セルフサービスによるパスワードのリセット (SSPR) に登録されているユーザーを抽出します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-137">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="6bef9-138">例: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-138">For example: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="6bef9-139">サポートされて`eq`いるフィルター演算子:。</span><span class="sxs-lookup"><span data-stu-id="6bef9-139">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="6bef9-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6bef9-140">isEnabled</span></span> | <span data-ttu-id="6bef9-141">SSPR に対して有効になっているユーザーを抽出します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-141">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="6bef9-142">例: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-142">For example: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="6bef9-143">サポートされて`eq`いる filtter 演算子:。</span><span class="sxs-lookup"><span data-stu-id="6bef9-143">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="6bef9-144">isCapable</span><span class="sxs-lookup"><span data-stu-id="6bef9-144">isCapable</span></span> | <span data-ttu-id="6bef9-145">パスワードのリセットまたは多要素認証 (MFA) を実行する準備ができているユーザーをフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-145">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="6bef9-146">例: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-146">For example: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="6bef9-147">サポートされているフィルター演算子:`eq`</span><span class="sxs-lookup"><span data-stu-id="6bef9-147">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="6bef9-148">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="6bef9-148">isMfaRegistered</span></span> | <span data-ttu-id="6bef9-149">MFA に登録されているユーザーを抽出します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-149">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="6bef9-150">例: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`。</span><span class="sxs-lookup"><span data-stu-id="6bef9-150">For example: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="6bef9-151">サポートされて`eq`いるフィルター演算子:。</span><span class="sxs-lookup"><span data-stu-id="6bef9-151">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6bef9-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6bef9-152">Request headers</span></span>

| <span data-ttu-id="6bef9-153">名前</span><span class="sxs-lookup"><span data-stu-id="6bef9-153">Name</span></span>      |<span data-ttu-id="6bef9-154">説明</span><span class="sxs-lookup"><span data-stu-id="6bef9-154">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6bef9-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bef9-155">Authorization</span></span> | <span data-ttu-id="6bef9-156">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="6bef9-156">Bearer {token}</span></span> |
| <span data-ttu-id="6bef9-157">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6bef9-157">Content-Type</span></span> | <span data-ttu-id="6bef9-158">application/json</span><span class="sxs-lookup"><span data-stu-id="6bef9-158">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bef9-159">要求本文</span><span class="sxs-lookup"><span data-stu-id="6bef9-159">Request body</span></span>

<span data-ttu-id="6bef9-160">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6bef9-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bef9-161">応答</span><span class="sxs-lookup"><span data-stu-id="6bef9-161">Response</span></span>

<span data-ttu-id="6bef9-162">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Credentialuserregistrationdetails](../resources/credentialuserregistrationdetails.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-162">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bef9-163">例</span><span class="sxs-lookup"><span data-stu-id="6bef9-163">Examples</span></span>

<span data-ttu-id="6bef9-164">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6bef9-164">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6bef9-165">要求</span><span class="sxs-lookup"><span data-stu-id="6bef9-165">Request</span></span>

<span data-ttu-id="6bef9-166">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6bef9-167">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6bef9-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6bef9-168">C#</span><span class="sxs-lookup"><span data-stu-id="6bef9-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bef9-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bef9-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6bef9-170">目的-C</span><span class="sxs-lookup"><span data-stu-id="6bef9-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6bef9-171">Java</span><span class="sxs-lookup"><span data-stu-id="6bef9-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bef9-172">応答</span><span class="sxs-lookup"><span data-stu-id="6bef9-172">Response</span></span>

<span data-ttu-id="6bef9-173">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6bef9-173">The following is an example of the response.</span></span>

> <span data-ttu-id="6bef9-174">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6bef9-174">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6bef9-175">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6bef9-175">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
