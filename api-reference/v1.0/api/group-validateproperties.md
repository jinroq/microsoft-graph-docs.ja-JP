---
title: 'グループ: validateProperties'
description: Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠していることを確認します。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 33844bd20b94868f91e2cb390b2dfaff830734ad
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932518"
---
# <a name="group-validateproperties"></a><span data-ttu-id="89186-103">グループ: validateProperties</span><span class="sxs-lookup"><span data-stu-id="89186-103">group: validateProperties</span></span>

<span data-ttu-id="89186-104">Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="89186-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="89186-105">クライアントは、この API を使用して、Office 365 グループの[更新](group-update.md)を試行する前に、表示名またはメールニックネームが有効かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="89186-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) an Office 365 group.</span></span> <span data-ttu-id="89186-106">グループを作成する前にプロパティを検証するには、 [directoryobject: validateProperties](directoryobject-validateproperties.md)関数を使用します。</span><span class="sxs-lookup"><span data-stu-id="89186-106">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="89186-107">[表示名] および [メールニックネーム] プロパティに対して、次のポリシー検証が実行されます。</span><span class="sxs-lookup"><span data-stu-id="89186-107">The following policy validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="89186-108">プレフィックスとサフィックスの名前付けポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="89186-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="89186-109">カスタムの禁止単語のポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="89186-109">Validate the custom banned words policy</span></span>

<span data-ttu-id="89186-110">この API は、検出された最初の検証エラーのみを返します。</span><span class="sxs-lookup"><span data-stu-id="89186-110">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="89186-111">プロパティが複数の検証に失敗した場合は、最初の検証エラーのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="89186-111">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="89186-112">ただし、プレフィックスとサフィックスの名前付けポリシーのみを検証する場合は、メールニックネームと表示名の両方を検証し、検証エラーのコレクションを受信することができます。</span><span class="sxs-lookup"><span data-stu-id="89186-112">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="89186-113">名前付けポリシーの構成の詳細については、「 [Configure ネーミング policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89186-113">To learn more about configuring naming policies, see [Configure naming policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="89186-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89186-114">Permissions</span></span>

<span data-ttu-id="89186-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89186-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89186-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89186-117">Permission type</span></span>      | <span data-ttu-id="89186-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89186-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89186-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89186-119">Delegated (work or school account)</span></span> | <span data-ttu-id="89186-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89186-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="89186-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89186-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89186-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89186-122">Not supported.</span></span>    |
|<span data-ttu-id="89186-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89186-123">Application</span></span> | <span data-ttu-id="89186-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89186-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89186-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89186-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="89186-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89186-126">Request headers</span></span>

| <span data-ttu-id="89186-127">名前</span><span class="sxs-lookup"><span data-stu-id="89186-127">Name</span></span>           | <span data-ttu-id="89186-128">説明</span><span class="sxs-lookup"><span data-stu-id="89186-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="89186-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="89186-129">Authorization</span></span>  | <span data-ttu-id="89186-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="89186-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="89186-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89186-132">Content-Type</span></span>   | <span data-ttu-id="89186-133">application/json</span><span class="sxs-lookup"><span data-stu-id="89186-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="89186-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="89186-134">Request body</span></span>

<span data-ttu-id="89186-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="89186-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="89186-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="89186-136">Parameter</span></span>    | <span data-ttu-id="89186-137">型</span><span class="sxs-lookup"><span data-stu-id="89186-137">Type</span></span>   |<span data-ttu-id="89186-138">説明</span><span class="sxs-lookup"><span data-stu-id="89186-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89186-139">displayName</span><span class="sxs-lookup"><span data-stu-id="89186-139">displayName</span></span>|<span data-ttu-id="89186-140">文字列</span><span class="sxs-lookup"><span data-stu-id="89186-140">String</span></span>| <span data-ttu-id="89186-141">検証するグループの表示名。</span><span class="sxs-lookup"><span data-stu-id="89186-141">The display name of the group to validate.</span></span> <span data-ttu-id="89186-142">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="89186-142">The property is not individually required.</span></span> <span data-ttu-id="89186-143">ただし、少なくとも1つのプロパティ (**displayName**または**mailNickname**) が必要です。</span><span class="sxs-lookup"><span data-stu-id="89186-143">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="89186-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="89186-144">mailNickname</span></span>|<span data-ttu-id="89186-145">String</span><span class="sxs-lookup"><span data-stu-id="89186-145">String</span></span>| <span data-ttu-id="89186-146">検証するグループのメールニックネーム。</span><span class="sxs-lookup"><span data-stu-id="89186-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="89186-147">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="89186-147">The property is not individually required.</span></span> <span data-ttu-id="89186-148">ただし、少なくとも1つのプロパティ (**displayName**または**mailNickname**) が必要です。</span><span class="sxs-lookup"><span data-stu-id="89186-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="89186-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="89186-149">onBehalfOfUserId</span></span>|<span data-ttu-id="89186-150">Guid</span><span class="sxs-lookup"><span data-stu-id="89186-150">Guid</span></span>| <span data-ttu-id="89186-151">API を呼び出すときに偽装するユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="89186-151">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="89186-152">検証結果は、 **onBehalfOfUserId の**属性とロールに対して行われます。</span><span class="sxs-lookup"><span data-stu-id="89186-152">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="89186-153">応答</span><span class="sxs-lookup"><span data-stu-id="89186-153">Response</span></span>
<span data-ttu-id="89186-154">成功した場合、検証エラーがない場合、メソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="89186-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="89186-155">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="89186-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="89186-156">要求が無効である場合、メソッドは`400 Bad Request`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="89186-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="89186-157">無効な要求に関する詳細を含むエラーメッセージが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="89186-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="89186-158">検証エラーが発生した場合。</span><span class="sxs-lookup"><span data-stu-id="89186-158">If there is a validation error.</span></span> <span data-ttu-id="89186-159">メソッドは応答`422 Unprocessable Entity`コードを返します。</span><span class="sxs-lookup"><span data-stu-id="89186-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="89186-160">エラーメッセージとエラーの詳細のコレクションが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="89186-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89186-161">例</span><span class="sxs-lookup"><span data-stu-id="89186-161">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="89186-162">例 1: 正常な検証要求</span><span class="sxs-lookup"><span data-stu-id="89186-162">Example 1: Successful validation request</span></span>
<span data-ttu-id="89186-163">これは、正常な検証要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89186-163">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="89186-164">要求</span><span class="sxs-lookup"><span data-stu-id="89186-164">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89186-165">プロトコル</span><span class="sxs-lookup"><span data-stu-id="89186-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89186-166">C#</span><span class="sxs-lookup"><span data-stu-id="89186-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89186-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="89186-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89186-168">目的-C</span><span class="sxs-lookup"><span data-stu-id="89186-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89186-169">Java</span><span class="sxs-lookup"><span data-stu-id="89186-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89186-170">応答</span><span class="sxs-lookup"><span data-stu-id="89186-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="89186-171">例 2: 検証エラーがある要求</span><span class="sxs-lookup"><span data-stu-id="89186-171">Example 2: Request with validation errors</span></span>
<span data-ttu-id="89186-172">これは、検証エラーが発生した要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89186-172">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="89186-173">要求</span><span class="sxs-lookup"><span data-stu-id="89186-173">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="89186-174">応答</span><span class="sxs-lookup"><span data-stu-id="89186-174">Response</span></span>
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
