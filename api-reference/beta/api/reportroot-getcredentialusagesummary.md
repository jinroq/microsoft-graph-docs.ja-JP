---
title: 'reportRoot: getCredentialUsageSummary'
description: 組織内のユーザーがセルフサービスのパスワードリセット機能を使用している現在の状態を報告します。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: ac704a7a710d0920813c73084923792c61844aac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308768"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="27d86-103">reportRoot: getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="27d86-103">reportRoot: getCredentialUsageSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d86-104">組織内のユーザーの数について、セルフサービスのパスワードのリセット機能を使用した現在の状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="27d86-104">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="27d86-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="27d86-105">Permissions</span></span>

<span data-ttu-id="27d86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27d86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27d86-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27d86-108">Permission type</span></span>                        | <span data-ttu-id="27d86-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="27d86-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27d86-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="27d86-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27d86-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27d86-111">Reports.Read.All</span></span> |
| <span data-ttu-id="27d86-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27d86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27d86-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27d86-113">Not supported.</span></span> |
| <span data-ttu-id="27d86-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27d86-114">Application</span></span>                            | <span data-ttu-id="27d86-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27d86-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27d86-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27d86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="27d86-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="27d86-117">Function parameters</span></span>

<span data-ttu-id="27d86-118">次の関数パラメーターを使用して、応答を調整できます。</span><span class="sxs-lookup"><span data-stu-id="27d86-118">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="27d86-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="27d86-119">Parameter</span></span> | <span data-ttu-id="27d86-120">型</span><span class="sxs-lookup"><span data-stu-id="27d86-120">Type</span></span> | <span data-ttu-id="27d86-121">説明</span><span class="sxs-lookup"><span data-stu-id="27d86-121">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="27d86-122">period</span><span class="sxs-lookup"><span data-stu-id="27d86-122">period</span></span> | <span data-ttu-id="27d86-123">String</span><span class="sxs-lookup"><span data-stu-id="27d86-123">String</span></span> | <span data-ttu-id="27d86-124">利用状況データを必要とする期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="27d86-124">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="27d86-125">例: `/reports/getCredentialUsageSummary(period='D30')`。</span><span class="sxs-lookup"><span data-stu-id="27d86-125">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="27d86-126">サポートされ`D1`て`D7`いる期間`D30`:、、。</span><span class="sxs-lookup"><span data-stu-id="27d86-126">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="27d86-127">ピリオドは大文字と小文字を区別しません。</span><span class="sxs-lookup"><span data-stu-id="27d86-127">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="27d86-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="27d86-128">Optional query parameters</span></span>

<span data-ttu-id="27d86-129">この関数は、オプションの OData クエリパラメーター **$filter**をサポートします。</span><span class="sxs-lookup"><span data-stu-id="27d86-129">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="27d86-130">[CredentialUsageSummary](../resources/credentialusagesummary.md)リソースの次の1つ以上のプロパティに **$filter**を適用できます。</span><span class="sxs-lookup"><span data-stu-id="27d86-130">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="27d86-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27d86-131">Properties</span></span> | <span data-ttu-id="27d86-132">説明と例</span><span class="sxs-lookup"><span data-stu-id="27d86-132">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="27d86-133">特徴</span><span class="sxs-lookup"><span data-stu-id="27d86-133">feature</span></span> | <span data-ttu-id="27d86-134">必要な利用状況データの種類 (登録とリセット) を指定します。</span><span class="sxs-lookup"><span data-stu-id="27d86-134">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="27d86-135">例: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`。</span><span class="sxs-lookup"><span data-stu-id="27d86-135">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="27d86-136">サポートされて`eq`いるフィルター演算子:。</span><span class="sxs-lookup"><span data-stu-id="27d86-136">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="27d86-137">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27d86-137">Request headers</span></span>

| <span data-ttu-id="27d86-138">名前</span><span class="sxs-lookup"><span data-stu-id="27d86-138">Name</span></span>          | <span data-ttu-id="27d86-139">説明</span><span class="sxs-lookup"><span data-stu-id="27d86-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27d86-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="27d86-140">Authorization</span></span> | <span data-ttu-id="27d86-141">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="27d86-141">Bearer {token}</span></span> |
| <span data-ttu-id="27d86-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27d86-142">Content-Type</span></span> | <span data-ttu-id="27d86-143">application/json</span><span class="sxs-lookup"><span data-stu-id="27d86-143">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="27d86-144">要求本文</span><span class="sxs-lookup"><span data-stu-id="27d86-144">Request body</span></span>

<span data-ttu-id="27d86-145">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="27d86-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27d86-146">応答</span><span class="sxs-lookup"><span data-stu-id="27d86-146">Response</span></span>

<span data-ttu-id="27d86-147">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で新しい[credentialUsageSummary](../resources/credentialusagesummary.md) collection オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27d86-147">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27d86-148">例</span><span class="sxs-lookup"><span data-stu-id="27d86-148">Examples</span></span>

<span data-ttu-id="27d86-149">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="27d86-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="27d86-150">要求</span><span class="sxs-lookup"><span data-stu-id="27d86-150">Request</span></span>

<span data-ttu-id="27d86-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="27d86-151">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27d86-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="27d86-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27d86-153">C#</span><span class="sxs-lookup"><span data-stu-id="27d86-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27d86-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d86-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27d86-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="27d86-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27d86-156">Java</span><span class="sxs-lookup"><span data-stu-id="27d86-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialusagesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27d86-157">応答</span><span class="sxs-lookup"><span data-stu-id="27d86-157">Response</span></span>

<span data-ttu-id="27d86-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="27d86-158">The following is an example of the response.</span></span>

> <span data-ttu-id="27d86-159">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="27d86-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="27d86-160">すべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27d86-160">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
