---
title: 'グループ: validateProperties'
description: Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠しているかどうかを検証します。 クライアントは API を使用して、Office 365 グループの**更新**を試行する前に、表示名またはメールニックネームが有効かどうかを判断します。 グループを作成する前にプロパティを検証するには、ディレクトリオブジェクトに対して validateProperties 関数を使用します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: dc1f156be72536e2765d77fefa09fe2f5c4bbeec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857743"
---
# <a name="group-validateproperties"></a><span data-ttu-id="fe0cf-105">グループ: validateProperties</span><span class="sxs-lookup"><span data-stu-id="fe0cf-105">group: validateProperties</span></span>

<span data-ttu-id="fe0cf-106">Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠しているかどうかを検証します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="fe0cf-107">クライアントは API を使用して、Office 365 グループの**更新**を試行する前に、表示名またはメールニックネームが有効かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="fe0cf-108">グループを作成する前にプロパティを検証するには、ディレクトリオブジェクトに対して[validateproperties 関数](directoryobject-validateproperties.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="fe0cf-109">[表示名] および [メールニックネーム] プロパティに対して、次の検証が実行されます。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="fe0cf-110">プレフィックスとサフィックスの名前付けポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="fe0cf-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="fe0cf-111">カスタムの禁止単語のポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="fe0cf-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="fe0cf-112">この API は、最初のエラーが発生したことを返します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="fe0cf-113">1つ以上のプロパティが複数の検証に失敗した場合、最初の検証に失敗したプロパティのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="fe0cf-114">ただし、プレフィックスとサフィックスの名前付けポリシーのみを検証する場合は、メールニックネームと表示名の両方を検証し、検証エラーのコレクションを受信することができます。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe0cf-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe0cf-115">Permissions</span></span>

<span data-ttu-id="fe0cf-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe0cf-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe0cf-118">Permission type</span></span>      | <span data-ttu-id="fe0cf-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe0cf-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe0cf-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe0cf-120">Delegated (work or school account)</span></span> | <span data-ttu-id="fe0cf-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe0cf-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe0cf-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe0cf-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe0cf-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-123">Not supported.</span></span>    |
|<span data-ttu-id="fe0cf-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe0cf-124">Application</span></span> | <span data-ttu-id="fe0cf-125">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe0cf-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe0cf-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe0cf-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="fe0cf-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe0cf-127">Request headers</span></span>

| <span data-ttu-id="fe0cf-128">名前</span><span class="sxs-lookup"><span data-stu-id="fe0cf-128">Name</span></span>           | <span data-ttu-id="fe0cf-129">説明</span><span class="sxs-lookup"><span data-stu-id="fe0cf-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="fe0cf-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe0cf-130">Authorization</span></span>  | <span data-ttu-id="fe0cf-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fe0cf-131">Bearer {code}</span></span>    |
| <span data-ttu-id="fe0cf-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe0cf-132">Content-Type</span></span>   | <span data-ttu-id="fe0cf-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fe0cf-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe0cf-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe0cf-134">Request body</span></span>

<span data-ttu-id="fe0cf-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe0cf-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe0cf-136">Parameter</span></span>    | <span data-ttu-id="fe0cf-137">型</span><span class="sxs-lookup"><span data-stu-id="fe0cf-137">Type</span></span>   |<span data-ttu-id="fe0cf-138">説明</span><span class="sxs-lookup"><span data-stu-id="fe0cf-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe0cf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fe0cf-139">displayName</span></span>|<span data-ttu-id="fe0cf-140">文字列</span><span class="sxs-lookup"><span data-stu-id="fe0cf-140">String</span></span>| <span data-ttu-id="fe0cf-141">検証するグループの表示名。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-141">The display name of the group to validate.</span></span> <span data-ttu-id="fe0cf-142">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-142">The property is not individually required.</span></span> <span data-ttu-id="fe0cf-143">ただし、少なくとも1つのプロパティ (displayName または mailNickname) が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="fe0cf-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="fe0cf-144">mailNickname</span></span>|<span data-ttu-id="fe0cf-145">String</span><span class="sxs-lookup"><span data-stu-id="fe0cf-145">String</span></span>| <span data-ttu-id="fe0cf-146">検証するグループのメールニックネーム。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="fe0cf-147">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-147">The property is not individually required.</span></span> <span data-ttu-id="fe0cf-148">ただし、少なくとも1つのプロパティ (displayName または mailNickname) が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="fe0cf-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="fe0cf-149">onBehalfOfUserId</span></span>|<span data-ttu-id="fe0cf-150">Guid</span><span class="sxs-lookup"><span data-stu-id="fe0cf-150">Guid</span></span>| <span data-ttu-id="fe0cf-151">API を呼び出すときに偽装するユーザーのオブジェクト ID。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="fe0cf-152">検証結果は、onBehalfOfUserId の属性とロールに対して行われます。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="fe0cf-153">応答</span><span class="sxs-lookup"><span data-stu-id="fe0cf-153">Response</span></span>
<span data-ttu-id="fe0cf-154">成功した場合、検証エラーがない場合、メソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="fe0cf-155">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="fe0cf-156">要求が無効である場合、メソッドは`400 Bad Request`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="fe0cf-157">無効な要求に関する詳細を含むエラーメッセージが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="fe0cf-158">検証エラーが発生した場合。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-158">If there is a validation error.</span></span> <span data-ttu-id="fe0cf-159">メソッドは応答`422 Unprocessable Entity`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="fe0cf-160">エラーメッセージとエラーの詳細のコレクションが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe0cf-161">例</span><span class="sxs-lookup"><span data-stu-id="fe0cf-161">Examples</span></span>

<span data-ttu-id="fe0cf-162">これは、正常な検証要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="fe0cf-163">要求</span><span class="sxs-lookup"><span data-stu-id="fe0cf-163">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe0cf-164">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fe0cf-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe0cf-165">C#</span><span class="sxs-lookup"><span data-stu-id="fe0cf-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe0cf-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe0cf-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe0cf-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="fe0cf-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fe0cf-168">Java</span><span class="sxs-lookup"><span data-stu-id="fe0cf-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe0cf-169">応答</span><span class="sxs-lookup"><span data-stu-id="fe0cf-169">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="fe0cf-170">これは、検証エラーが発生した要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe0cf-170">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="fe0cf-171">要求</span><span class="sxs-lookup"><span data-stu-id="fe0cf-171">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="fe0cf-172">応答</span><span class="sxs-lookup"><span data-stu-id="fe0cf-172">Response</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
