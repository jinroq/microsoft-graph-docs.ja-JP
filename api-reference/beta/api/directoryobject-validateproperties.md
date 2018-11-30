---
title: 'directoryObject: validateProperties'
description: Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。  クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を作成**する前に、メールのニックネームが無効です。 既存のグループのプロパティを検証するためには、グループの validateProperties 関数を使用します。
ms.openlocfilehash: 82592eff14829fdd8ae1d74c87f43402a3938adf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067924"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="bf954-105">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="bf954-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="bf954-106">Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。</span><span class="sxs-lookup"><span data-stu-id="bf954-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="bf954-107">クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を作成**する前に、メールのニックネームが無効です。</span><span class="sxs-lookup"><span data-stu-id="bf954-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="bf954-108">既存のグループのプロパティを検証するためには、グループの[validateProperties 関数](group-validateproperties.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="bf954-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="bf954-109">表示名とメールのニックネームのプロパティには、次の検証が実行されます。</span><span class="sxs-lookup"><span data-stu-id="bf954-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="bf954-110">プリフィックスおよびサフィックスの名前付けポリシーを検証します。</span><span class="sxs-lookup"><span data-stu-id="bf954-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="bf954-111">禁止された単語をカスタム ポリシーを検証します。</span><span class="sxs-lookup"><span data-stu-id="bf954-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="bf954-112">検証、メールのニックネームが一意では</span><span class="sxs-lookup"><span data-stu-id="bf954-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="bf954-113">この API は、最初のエラーが発生しましたを返します。</span><span class="sxs-lookup"><span data-stu-id="bf954-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="bf954-114">1 つまたは複数のプロパティには、複数の検証が失敗した場合、最初の検証エラーのプロパティだけが返されます。</span><span class="sxs-lookup"><span data-stu-id="bf954-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="bf954-115">ただし、メールのニックネームと表示名の両方を検証し、検証エラーのコレクションが表示される場合は、プレフィックスとサフィックスの名前付けポリシーを検証しているだけです。</span><span class="sxs-lookup"><span data-stu-id="bf954-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf954-116">前提条件</span><span class="sxs-lookup"><span data-stu-id="bf954-116">Prerequisites</span></span>

<span data-ttu-id="bf954-117">この API を実行するために次の**アクセス許可**が必要です: *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="bf954-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="bf954-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf954-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="bf954-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf954-119">Request headers</span></span>

| <span data-ttu-id="bf954-120">名前</span><span class="sxs-lookup"><span data-stu-id="bf954-120">Name</span></span>           | <span data-ttu-id="bf954-121">説明</span><span class="sxs-lookup"><span data-stu-id="bf954-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="bf954-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf954-122">Authorization</span></span>  | <span data-ttu-id="bf954-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bf954-123">Bearer {code}</span></span>    |
| <span data-ttu-id="bf954-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf954-124">Content-Type</span></span>   | <span data-ttu-id="bf954-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf954-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf954-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf954-126">Request body</span></span>
<span data-ttu-id="bf954-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bf954-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf954-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bf954-128">Parameter</span></span>    | <span data-ttu-id="bf954-129">型</span><span class="sxs-lookup"><span data-stu-id="bf954-129">Type</span></span>   |<span data-ttu-id="bf954-130">説明</span><span class="sxs-lookup"><span data-stu-id="bf954-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf954-131">entityType</span><span class="sxs-lookup"><span data-stu-id="bf954-131">entityType</span></span>|<span data-ttu-id="bf954-132">String</span><span class="sxs-lookup"><span data-stu-id="bf954-132">String</span></span>| <span data-ttu-id="bf954-133">`Group`唯一サポートされているエンティティの種類です。</span><span class="sxs-lookup"><span data-stu-id="bf954-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="bf954-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bf954-134">displayName</span></span>|<span data-ttu-id="bf954-135">String</span><span class="sxs-lookup"><span data-stu-id="bf954-135">String</span></span>| <span data-ttu-id="bf954-136">検証グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="bf954-136">The display name of the group to validate.</span></span> <span data-ttu-id="bf954-137">プロパティは、個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="bf954-137">The property is not individually required.</span></span> <span data-ttu-id="bf954-138">ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf954-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="bf954-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bf954-139">mailNickname</span></span>|<span data-ttu-id="bf954-140">String</span><span class="sxs-lookup"><span data-stu-id="bf954-140">String</span></span>| <span data-ttu-id="bf954-141">検証するためにグループのメール ニックネーム。</span><span class="sxs-lookup"><span data-stu-id="bf954-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="bf954-142">プロパティは、個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="bf954-142">The property is not individually required.</span></span> <span data-ttu-id="bf954-143">ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf954-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="bf954-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="bf954-144">onBehalfOfUserId</span></span>|<span data-ttu-id="bf954-145">Guid</span><span class="sxs-lookup"><span data-stu-id="bf954-145">Guid</span></span>| <span data-ttu-id="bf954-146">API を呼び出すときに偽装するユーザーのオブジェクト ID です。</span><span class="sxs-lookup"><span data-stu-id="bf954-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="bf954-147">検証の結果は、onBehalfOfUserId の属性とロールのです。</span><span class="sxs-lookup"><span data-stu-id="bf954-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="bf954-148">応答</span><span class="sxs-lookup"><span data-stu-id="bf954-148">Response</span></span>

<span data-ttu-id="bf954-149">正常終了した場合、検証エラーは、メソッドを返します`204 No Content`応答コード。</span><span class="sxs-lookup"><span data-stu-id="bf954-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="bf954-150">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="bf954-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="bf954-151">メソッドを返すかどうか、要求が有効でない`400 Bad Request`応答コード。</span><span class="sxs-lookup"><span data-stu-id="bf954-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="bf954-152">応答本体には、無効な要求に関する詳細情報をエラー メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="bf954-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="bf954-153">メソッドを返すかどうかは検証エラーがある場合、`422 Unprocessable Entity`応答コード。</span><span class="sxs-lookup"><span data-stu-id="bf954-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="bf954-154">応答本体には、エラー メッセージとエラーの詳細情報のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="bf954-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf954-155">例</span><span class="sxs-lookup"><span data-stu-id="bf954-155">Examples</span></span>

<span data-ttu-id="bf954-156">これは、検証が成功した要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf954-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="bf954-157">要求</span><span class="sxs-lookup"><span data-stu-id="bf954-157">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="bf954-158">応答</span><span class="sxs-lookup"><span data-stu-id="bf954-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="bf954-159">これは、要求の妥当性確認エラーの例です。</span><span class="sxs-lookup"><span data-stu-id="bf954-159">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="bf954-160">要求</span><span class="sxs-lookup"><span data-stu-id="bf954-160">Request</span></span>
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="bf954-161">応答</span><span class="sxs-lookup"><span data-stu-id="bf954-161">Response</span></span>
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
  "tocPath": ""
}-->
