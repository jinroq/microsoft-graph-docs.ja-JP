---
title: 'グループ: validateProperties'
description: Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。 クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を更新**する前に、メールのニックネームが無効です。 プロパティを検証グループを作成する前に、ディレクトリ オブジェクトの validateProperties 関数を使用します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5361e05d2a58e2d4c27bd662f158d4f185c447fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990891"
---
# <a name="group-validateproperties"></a><span data-ttu-id="b4b2f-105">グループ: validateProperties</span><span class="sxs-lookup"><span data-stu-id="b4b2f-105">group: validateProperties</span></span>

<span data-ttu-id="b4b2f-106">Office 365 のグループの表示名やメールのニックネームは、命名ポリシーに準拠している場合を検証します。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="b4b2f-107">クライアントは、API を使用して場合は、表示名を確認または、Office 365 のグループ**を更新**する前に、メールのニックネームが無効です。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="b4b2f-108">プロパティを検証グループを作成する前に、ディレクトリ オブジェクトの[validateProperties 関数](directoryobject-validateproperties.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="b4b2f-109">表示名とメールのニックネームのプロパティには、次の検証が実行されます。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="b4b2f-110">プリフィックスおよびサフィックスの名前付けポリシーを検証します。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="b4b2f-111">禁止された単語をカスタム ポリシーを検証します。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="b4b2f-112">この API は、最初のエラーが発生しましたを返します。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="b4b2f-113">1 つまたは複数のプロパティには、複数の検証が失敗した場合、最初の検証エラーのプロパティだけが返されます。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="b4b2f-114">ただし、メールのニックネームと表示名の両方を検証し、検証エラーのコレクションが表示される場合は、プレフィックスとサフィックスの名前付けポリシーを検証しているだけです。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4b2f-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4b2f-115">Permissions</span></span>

<span data-ttu-id="b4b2f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b2f-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4b2f-118">Permission type</span></span>      | <span data-ttu-id="b4b2f-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4b2f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4b2f-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4b2f-120">Delegated (work or school account)</span></span> | <span data-ttu-id="b4b2f-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b2f-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4b2f-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4b2f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4b2f-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-123">Not supported.</span></span>    |
|<span data-ttu-id="b4b2f-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4b2f-124">Application</span></span> | <span data-ttu-id="b4b2f-125">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4b2f-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4b2f-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4b2f-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="b4b2f-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4b2f-127">Request headers</span></span>

| <span data-ttu-id="b4b2f-128">名前</span><span class="sxs-lookup"><span data-stu-id="b4b2f-128">Name</span></span>           | <span data-ttu-id="b4b2f-129">説明</span><span class="sxs-lookup"><span data-stu-id="b4b2f-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="b4b2f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4b2f-130">Authorization</span></span>  | <span data-ttu-id="b4b2f-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b4b2f-131">Bearer {code}</span></span>    |
| <span data-ttu-id="b4b2f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4b2f-132">Content-Type</span></span>   | <span data-ttu-id="b4b2f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b2f-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4b2f-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4b2f-134">Request body</span></span>

<span data-ttu-id="b4b2f-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4b2f-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b4b2f-136">Parameter</span></span>    | <span data-ttu-id="b4b2f-137">Type</span><span class="sxs-lookup"><span data-stu-id="b4b2f-137">Type</span></span>   |<span data-ttu-id="b4b2f-138">説明</span><span class="sxs-lookup"><span data-stu-id="b4b2f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4b2f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b4b2f-139">displayName</span></span>|<span data-ttu-id="b4b2f-140">String</span><span class="sxs-lookup"><span data-stu-id="b4b2f-140">String</span></span>| <span data-ttu-id="b4b2f-141">検証グループの表示名。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-141">The display name of the group to validate.</span></span> <span data-ttu-id="b4b2f-142">プロパティは、個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-142">The property is not individually required.</span></span> <span data-ttu-id="b4b2f-143">ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="b4b2f-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b4b2f-144">mailNickname</span></span>|<span data-ttu-id="b4b2f-145">String</span><span class="sxs-lookup"><span data-stu-id="b4b2f-145">String</span></span>| <span data-ttu-id="b4b2f-146">検証するためにグループのメール ニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="b4b2f-147">プロパティは、個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-147">The property is not individually required.</span></span> <span data-ttu-id="b4b2f-148">ただし、少なくとも 1 つのプロパティ (表示名または mailNickname) は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="b4b2f-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="b4b2f-149">onBehalfOfUserId</span></span>|<span data-ttu-id="b4b2f-150">Guid</span><span class="sxs-lookup"><span data-stu-id="b4b2f-150">Guid</span></span>| <span data-ttu-id="b4b2f-151">API を呼び出すときに偽装するユーザーのオブジェクト ID です。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="b4b2f-152">検証の結果は、onBehalfOfUserId の属性とロールのです。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="b4b2f-153">応答</span><span class="sxs-lookup"><span data-stu-id="b4b2f-153">Response</span></span>
<span data-ttu-id="b4b2f-154">正常終了した場合、検証エラーは、メソッドを返します`204 No Content`応答コード。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="b4b2f-155">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="b4b2f-156">メソッドを返すかどうか、要求が有効でない`400 Bad Request`応答コード。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="b4b2f-157">応答本体には、無効な要求に関する詳細情報をエラー メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="b4b2f-158">検証エラーがある場合。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-158">If there is a validation error.</span></span> <span data-ttu-id="b4b2f-159">メソッドが返す`422 Unprocessable Entity`応答コード。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="b4b2f-160">応答本体には、エラー メッセージとエラーの詳細情報のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4b2f-161">例</span><span class="sxs-lookup"><span data-stu-id="b4b2f-161">Examples</span></span>

<span data-ttu-id="b4b2f-162">これは、検証が成功した要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="b4b2f-163">要求</span><span class="sxs-lookup"><span data-stu-id="b4b2f-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="b4b2f-164">応答</span><span class="sxs-lookup"><span data-stu-id="b4b2f-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="b4b2f-165">これは、要求の妥当性確認エラーの例です。</span><span class="sxs-lookup"><span data-stu-id="b4b2f-165">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="b4b2f-166">要求</span><span class="sxs-lookup"><span data-stu-id="b4b2f-166">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="b4b2f-167">応答</span><span class="sxs-lookup"><span data-stu-id="b4b2f-167">Response</span></span>
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
