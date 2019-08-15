---
title: 'directoryObject: validateProperties'
description: Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠しているかどうかを検証します。  クライアントは API を使用して、Office 365 グループを**作成**する前に、表示名またはメールニックネームが有効かどうかを判断します。 既存のグループのプロパティを検証するには、グループに対して validateProperties 関数を使用します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b701021143cbe8fe8193fbdaa21ad8b815de1b5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417341"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="7bc0d-105">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="7bc0d-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="7bc0d-106">Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠しているかどうかを検証します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="7bc0d-107">クライアントは API を使用して、Office 365 グループを**作成**する前に、表示名またはメールニックネームが有効かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="7bc0d-108">既存のグループのプロパティを検証するには、グループに対して[validateproperties 関数](group-validateproperties.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="7bc0d-109">[表示名] および [メールニックネーム] プロパティに対して、次の検証が実行されます。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="7bc0d-110">プレフィックスとサフィックスの名前付けポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="7bc0d-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="7bc0d-111">カスタムの禁止単語のポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="7bc0d-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="7bc0d-112">メールニックネームが一意であることを確認する</span><span class="sxs-lookup"><span data-stu-id="7bc0d-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="7bc0d-113">この API は、最初のエラーが発生したことを返します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="7bc0d-114">1つ以上のプロパティが複数の検証に失敗した場合、最初の検証に失敗したプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="7bc0d-115">ただし、プレフィックスとサフィックスの名前付けポリシーのみを検証する場合は、メールニックネームと表示名の両方を検証し、検証エラーのコレクションを受信することができます。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bc0d-116">前提条件</span><span class="sxs-lookup"><span data-stu-id="7bc0d-116">Prerequisites</span></span>

<span data-ttu-id="7bc0d-117">この API を実行するには、次の\*\* **アクセス許可**が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="7bc0d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bc0d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="7bc0d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bc0d-119">Request headers</span></span>

| <span data-ttu-id="7bc0d-120">名前</span><span class="sxs-lookup"><span data-stu-id="7bc0d-120">Name</span></span>           | <span data-ttu-id="7bc0d-121">説明</span><span class="sxs-lookup"><span data-stu-id="7bc0d-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="7bc0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bc0d-122">Authorization</span></span>  | <span data-ttu-id="7bc0d-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7bc0d-123">Bearer {code}</span></span>    |
| <span data-ttu-id="7bc0d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bc0d-124">Content-Type</span></span>   | <span data-ttu-id="7bc0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7bc0d-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bc0d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7bc0d-126">Request body</span></span>
<span data-ttu-id="7bc0d-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7bc0d-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7bc0d-128">Parameter</span></span>    | <span data-ttu-id="7bc0d-129">型</span><span class="sxs-lookup"><span data-stu-id="7bc0d-129">Type</span></span>   |<span data-ttu-id="7bc0d-130">説明</span><span class="sxs-lookup"><span data-stu-id="7bc0d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bc0d-131">entityType</span><span class="sxs-lookup"><span data-stu-id="7bc0d-131">entityType</span></span>|<span data-ttu-id="7bc0d-132">String</span><span class="sxs-lookup"><span data-stu-id="7bc0d-132">String</span></span>| <span data-ttu-id="7bc0d-133">`Group`は、サポートされている唯一のエンティティの種類です。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="7bc0d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7bc0d-134">displayName</span></span>|<span data-ttu-id="7bc0d-135">文字列</span><span class="sxs-lookup"><span data-stu-id="7bc0d-135">String</span></span>| <span data-ttu-id="7bc0d-136">検証するグループの表示名。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-136">The display name of the group to validate.</span></span> <span data-ttu-id="7bc0d-137">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-137">The property is not individually required.</span></span> <span data-ttu-id="7bc0d-138">ただし、少なくとも1つのプロパティ (displayName または mailNickname) が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="7bc0d-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7bc0d-139">mailNickname</span></span>|<span data-ttu-id="7bc0d-140">String</span><span class="sxs-lookup"><span data-stu-id="7bc0d-140">String</span></span>| <span data-ttu-id="7bc0d-141">検証するグループのメールニックネーム。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="7bc0d-142">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-142">The property is not individually required.</span></span> <span data-ttu-id="7bc0d-143">ただし、少なくとも1つのプロパティ (displayName または mailNickname) が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="7bc0d-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="7bc0d-144">onBehalfOfUserId</span></span>|<span data-ttu-id="7bc0d-145">Guid</span><span class="sxs-lookup"><span data-stu-id="7bc0d-145">Guid</span></span>| <span data-ttu-id="7bc0d-146">API を呼び出すときに偽装するユーザーのオブジェクト ID。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="7bc0d-147">検証結果は、onBehalfOfUserId の属性とロールに対して行われます。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="7bc0d-148">応答</span><span class="sxs-lookup"><span data-stu-id="7bc0d-148">Response</span></span>

<span data-ttu-id="7bc0d-149">成功した場合、検証エラーがない場合、メソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="7bc0d-150">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="7bc0d-151">要求が無効である場合、メソッドは`400 Bad Request`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="7bc0d-152">無効な要求に関する詳細を含むエラーメッセージが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="7bc0d-153">検証エラーが発生した場合、メソッドは`422 Unprocessable Entity`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="7bc0d-154">エラーメッセージとエラーの詳細のコレクションが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bc0d-155">例</span><span class="sxs-lookup"><span data-stu-id="7bc0d-155">Examples</span></span>

<span data-ttu-id="7bc0d-156">これは、正常な検証要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="7bc0d-157">要求</span><span class="sxs-lookup"><span data-stu-id="7bc0d-157">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7bc0d-158">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7bc0d-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bc0d-159">C#</span><span class="sxs-lookup"><span data-stu-id="7bc0d-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc0d-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bc0d-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bc0d-161">目的-C</span><span class="sxs-lookup"><span data-stu-id="7bc0d-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bc0d-162">応答</span><span class="sxs-lookup"><span data-stu-id="7bc0d-162">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="7bc0d-163">これは、検証エラーが発生した要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7bc0d-163">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="7bc0d-164">要求</span><span class="sxs-lookup"><span data-stu-id="7bc0d-164">Request</span></span>
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="7bc0d-165">応答</span><span class="sxs-lookup"><span data-stu-id="7bc0d-165">Response</span></span>
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
