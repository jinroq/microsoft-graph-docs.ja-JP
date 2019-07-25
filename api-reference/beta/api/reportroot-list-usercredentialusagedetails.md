---
title: Usercredentialの詳細を一覧表示する
description: 指定したテナントの Usercredentialの詳細オブジェクトの一覧を取得します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 1ea46387a4d4f4c0920a94a2d082a20090fe0bb0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871232"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="08002-103">Usercredentialの詳細を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="08002-103">List userCredentialUsageDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08002-104">指定したテナントの[Usercredentialの詳細](../resources/usercredentialusagedetails.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="08002-104">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="08002-105">詳細には、ユーザー情報、リセットの状態、およびエラーの理由が含まれます。</span><span class="sxs-lookup"><span data-stu-id="08002-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="08002-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08002-106">Permissions</span></span>

<span data-ttu-id="08002-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08002-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08002-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08002-109">Permission type</span></span>                        | <span data-ttu-id="08002-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08002-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08002-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="08002-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08002-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08002-112">Reports.Read.All</span></span> |
| <span data-ttu-id="08002-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08002-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08002-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08002-114">Not supported.</span></span> |
| <span data-ttu-id="08002-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08002-115">Application</span></span>                            | <span data-ttu-id="08002-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="08002-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08002-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08002-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08002-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="08002-118">Optional query parameters</span></span>

<span data-ttu-id="08002-119">この関数は、オプションの OData クエリパラメーター **$filter**をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08002-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="08002-120">[Usercredentialの詳細](../resources/usercredentialusagedetails.md)リソースの次のプロパティの1つ以上に **$filter**を適用できます。</span><span class="sxs-lookup"><span data-stu-id="08002-120">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="08002-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08002-121">Properties</span></span> | <span data-ttu-id="08002-122">説明と例</span><span class="sxs-lookup"><span data-stu-id="08002-122">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="08002-123">特徴</span><span class="sxs-lookup"><span data-stu-id="08002-123">feature</span></span> | <span data-ttu-id="08002-124">必要な利用状況データの種類 (登録とリセット) によってフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="08002-124">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="08002-125">例: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`。</span><span class="sxs-lookup"><span data-stu-id="08002-125">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="08002-126">サポートされているフィルター演算子:`eq`</span><span class="sxs-lookup"><span data-stu-id="08002-126">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="08002-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="08002-127">userDisplayName</span></span> | <span data-ttu-id="08002-128">ユーザーの表示名でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="08002-128">Filter by user display name.</span></span> <span data-ttu-id="08002-129">例: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="08002-129">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="08002-130">サポートされて`eq`いる`startswith()`フィルター演算子: および。</span><span class="sxs-lookup"><span data-stu-id="08002-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="08002-131">大文字小文字の区別をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08002-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="08002-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08002-132">userPrincipalName</span></span>  | <span data-ttu-id="08002-133">ユーザープリンシパル名でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="08002-133">Filter by user principal name.</span></span> <span data-ttu-id="08002-134">例: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="08002-134">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="08002-135">サポートされて`eq`いる`startswith()`フィルター演算子: および。</span><span class="sxs-lookup"><span data-stu-id="08002-135">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="08002-136">大文字小文字の区別をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08002-136">Supports case insensitive.</span></span> |
| <span data-ttu-id="08002-137">この</span><span class="sxs-lookup"><span data-stu-id="08002-137">isSuccess</span></span> | <span data-ttu-id="08002-138">アクティビティの状態によってフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="08002-138">Filter by status of the activity.</span></span> <span data-ttu-id="08002-139">例: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`。</span><span class="sxs-lookup"><span data-stu-id="08002-139">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="08002-140">サポートされて`eq`いる`orderby`フィルター演算子: および。</span><span class="sxs-lookup"><span data-stu-id="08002-140">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="08002-141">authMethod</span><span class="sxs-lookup"><span data-stu-id="08002-141">authMethod</span></span>  | <span data-ttu-id="08002-142">登録時にを使用して、認証方法によってフィルター処理を行います。</span><span class="sxs-lookup"><span data-stu-id="08002-142">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="08002-143">例: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`。</span><span class="sxs-lookup"><span data-stu-id="08002-143">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="08002-144">サポートされて`eq`いるフィルター演算子:。</span><span class="sxs-lookup"><span data-stu-id="08002-144">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="08002-145">failureReason</span><span class="sxs-lookup"><span data-stu-id="08002-145">failureReason</span></span> | <span data-ttu-id="08002-146">失敗の理由 (アクティビティが失敗した場合) でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="08002-146">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="08002-147">例: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`。</span><span class="sxs-lookup"><span data-stu-id="08002-147">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="08002-148">サポートされて`eq`いる`startswith()`フィルター演算子: および。</span><span class="sxs-lookup"><span data-stu-id="08002-148">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="08002-149">大文字小文字の区別をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08002-149">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="08002-150">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08002-150">Request headers</span></span>

| <span data-ttu-id="08002-151">名前</span><span class="sxs-lookup"><span data-stu-id="08002-151">Name</span></span>      |<span data-ttu-id="08002-152">説明</span><span class="sxs-lookup"><span data-stu-id="08002-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08002-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="08002-153">Authorization</span></span> | <span data-ttu-id="08002-154">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="08002-154">Bearer {token}</span></span> |
| <span data-ttu-id="08002-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08002-155">Content-Type</span></span> | <span data-ttu-id="08002-156">application/json</span><span class="sxs-lookup"><span data-stu-id="08002-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08002-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="08002-157">Request body</span></span>

<span data-ttu-id="08002-158">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08002-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08002-159">応答</span><span class="sxs-lookup"><span data-stu-id="08002-159">Response</span></span>

<span data-ttu-id="08002-160">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Usercredentialの details](../resources/usercredentialusagedetails.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="08002-160">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08002-161">例</span><span class="sxs-lookup"><span data-stu-id="08002-161">Examples</span></span>

<span data-ttu-id="08002-162">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="08002-162">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="08002-163">要求</span><span class="sxs-lookup"><span data-stu-id="08002-163">Request</span></span>

<span data-ttu-id="08002-164">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08002-164">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08002-165">プロトコル</span><span class="sxs-lookup"><span data-stu-id="08002-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08002-166">C#</span><span class="sxs-lookup"><span data-stu-id="08002-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08002-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="08002-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08002-168">目的-C</span><span class="sxs-lookup"><span data-stu-id="08002-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08002-169">Java</span><span class="sxs-lookup"><span data-stu-id="08002-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08002-170">応答</span><span class="sxs-lookup"><span data-stu-id="08002-170">Response</span></span>

<span data-ttu-id="08002-171">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08002-171">The following is an example of the response.</span></span>

> <span data-ttu-id="08002-172">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="08002-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="08002-173">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08002-173">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 258

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
