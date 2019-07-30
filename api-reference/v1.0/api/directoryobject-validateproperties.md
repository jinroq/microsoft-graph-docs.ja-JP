---
title: 'directoryObject: validateProperties'
description: Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠していることを確認します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f26857514ec180dbbc50c73eeb8eccc4b30185ed
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932215"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="7593f-103">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="7593f-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="7593f-104">Office 365 グループの表示名またはメールニックネームが名前付けポリシーに準拠していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7593f-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="7593f-105">クライアントは、この API を使用して、Office 365 グループを[作成](group-post-groups.md)する前に、表示名またはメールニックネームが有効かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="7593f-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) an Office 365 group.</span></span> <span data-ttu-id="7593f-106">既存のグループのプロパティを検証するには、 [group: validateProperties](group-validateproperties.md)関数を使用します。</span><span class="sxs-lookup"><span data-stu-id="7593f-106">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="7593f-107">[表示名] および [メールニックネーム] プロパティに対して、次のポリシー検証が実行されます。</span><span class="sxs-lookup"><span data-stu-id="7593f-107">The following policy validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="7593f-108">プレフィックスとサフィックスの名前付けポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="7593f-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="7593f-109">カスタムの禁止単語のポリシーを検証する</span><span class="sxs-lookup"><span data-stu-id="7593f-109">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="7593f-110">メールニックネームが一意であることを確認する</span><span class="sxs-lookup"><span data-stu-id="7593f-110">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="7593f-111">この API は、検出された最初の検証エラーのみを返します。</span><span class="sxs-lookup"><span data-stu-id="7593f-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="7593f-112">プロパティが複数の検証に失敗した場合は、最初の検証エラーのみが返されます。</span><span class="sxs-lookup"><span data-stu-id="7593f-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="7593f-113">ただし、プレフィックスとサフィックスの名前付けポリシーのみを検証する場合は、メールニックネームと表示名の両方を検証し、検証エラーのコレクションを受信することができます。</span><span class="sxs-lookup"><span data-stu-id="7593f-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="7593f-114">名前付けポリシーの構成の詳細については、「 [Configure ネーミング policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7593f-114">To learn more about configuring naming policies, see [Configure naming policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="7593f-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7593f-115">Permissions</span></span>
<span data-ttu-id="7593f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7593f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7593f-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7593f-118">Permission type</span></span>      | <span data-ttu-id="7593f-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7593f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7593f-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7593f-120">Delegated (work or school account)</span></span> | <span data-ttu-id="7593f-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7593f-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7593f-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7593f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7593f-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7593f-123">Not supported.</span></span>    |
|<span data-ttu-id="7593f-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7593f-124">Application</span></span> | <span data-ttu-id="7593f-125">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7593f-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7593f-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7593f-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="7593f-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7593f-127">Request headers</span></span>

| <span data-ttu-id="7593f-128">名前</span><span class="sxs-lookup"><span data-stu-id="7593f-128">Name</span></span>           | <span data-ttu-id="7593f-129">説明</span><span class="sxs-lookup"><span data-stu-id="7593f-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="7593f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7593f-130">Authorization</span></span>  | <span data-ttu-id="7593f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7593f-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="7593f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7593f-133">Content-Type</span></span>   | <span data-ttu-id="7593f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="7593f-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7593f-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="7593f-135">Request body</span></span>
<span data-ttu-id="7593f-136">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7593f-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7593f-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7593f-137">Parameter</span></span>    | <span data-ttu-id="7593f-138">型</span><span class="sxs-lookup"><span data-stu-id="7593f-138">Type</span></span>   |<span data-ttu-id="7593f-139">説明</span><span class="sxs-lookup"><span data-stu-id="7593f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7593f-140">entityType</span><span class="sxs-lookup"><span data-stu-id="7593f-140">entityType</span></span>|<span data-ttu-id="7593f-141">String</span><span class="sxs-lookup"><span data-stu-id="7593f-141">String</span></span>| <span data-ttu-id="7593f-142">Group は、サポートされている唯一のエンティティの種類です。</span><span class="sxs-lookup"><span data-stu-id="7593f-142">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="7593f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7593f-143">displayName</span></span>|<span data-ttu-id="7593f-144">文字列</span><span class="sxs-lookup"><span data-stu-id="7593f-144">String</span></span>| <span data-ttu-id="7593f-145">検証するグループの表示名。</span><span class="sxs-lookup"><span data-stu-id="7593f-145">The display name of the group to validate.</span></span> <span data-ttu-id="7593f-146">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="7593f-146">The property is not individually required.</span></span> <span data-ttu-id="7593f-147">ただし、少なくとも1つのプロパティ (**displayName**または**mailNickname**) が必要です。</span><span class="sxs-lookup"><span data-stu-id="7593f-147">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="7593f-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7593f-148">mailNickname</span></span>|<span data-ttu-id="7593f-149">String</span><span class="sxs-lookup"><span data-stu-id="7593f-149">String</span></span>| <span data-ttu-id="7593f-150">検証するグループのメールニックネーム。</span><span class="sxs-lookup"><span data-stu-id="7593f-150">The mail nickname of the group to validate.</span></span> <span data-ttu-id="7593f-151">プロパティが個別に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="7593f-151">The property is not individually required.</span></span> <span data-ttu-id="7593f-152">ただし、少なくとも1つのプロパティ (**displayName**または**mailNickname**) が必要です。</span><span class="sxs-lookup"><span data-stu-id="7593f-152">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="7593f-153">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="7593f-153">onBehalfOfUserId</span></span>|<span data-ttu-id="7593f-154">Guid</span><span class="sxs-lookup"><span data-stu-id="7593f-154">Guid</span></span>| <span data-ttu-id="7593f-155">API を呼び出すときに偽装するユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="7593f-155">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="7593f-156">検証結果は、 **onBehalfOfUserId の**属性とロールに対して行われます。</span><span class="sxs-lookup"><span data-stu-id="7593f-156">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="7593f-157">応答</span><span class="sxs-lookup"><span data-stu-id="7593f-157">Response</span></span>

<span data-ttu-id="7593f-158">成功した場合、検証エラーがない場合、メソッド`204 No Content`は応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7593f-158">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="7593f-159">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7593f-159">It does not return anything in the response body.</span></span>

<span data-ttu-id="7593f-160">要求が無効である場合、メソッドは`400 Bad Request`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7593f-160">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="7593f-161">無効な要求に関する詳細を含むエラーメッセージが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="7593f-161">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="7593f-162">検証エラーが発生した場合、メソッドは`422 Unprocessable Entity`応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7593f-162">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="7593f-163">エラーメッセージとエラーの詳細のコレクションが応答本文で返されます。</span><span class="sxs-lookup"><span data-stu-id="7593f-163">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7593f-164">例</span><span class="sxs-lookup"><span data-stu-id="7593f-164">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="7593f-165">例 1: 正常な検証要求</span><span class="sxs-lookup"><span data-stu-id="7593f-165">Example 1: Successful validation request</span></span>
<span data-ttu-id="7593f-166">これは、正常な検証要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7593f-166">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="7593f-167">要求</span><span class="sxs-lookup"><span data-stu-id="7593f-167">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7593f-168">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7593f-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7593f-169">C#</span><span class="sxs-lookup"><span data-stu-id="7593f-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7593f-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="7593f-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7593f-171">目的-C</span><span class="sxs-lookup"><span data-stu-id="7593f-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7593f-172">Java</span><span class="sxs-lookup"><span data-stu-id="7593f-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7593f-173">応答</span><span class="sxs-lookup"><span data-stu-id="7593f-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="7593f-174">例 2: 検証エラーがある要求</span><span class="sxs-lookup"><span data-stu-id="7593f-174">Example 2: Request with validation errors</span></span>
<span data-ttu-id="7593f-175">これは、検証エラーが発生した要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7593f-175">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="7593f-176">要求</span><span class="sxs-lookup"><span data-stu-id="7593f-176">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

#### <a name="response"></a><span data-ttu-id="7593f-177">応答</span><span class="sxs-lookup"><span data-stu-id="7593f-177">Response</span></span>
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
