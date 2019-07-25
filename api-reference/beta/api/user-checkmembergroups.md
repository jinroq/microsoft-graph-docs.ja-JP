---
title: checkMemberGroups
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 41da2d19044bb55fd5ebf8e18c31b267afc3b895
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867900"
---
# <a name="checkmembergroups"></a><span data-ttu-id="d62d4-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d62d4-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d62d4-p102">指定したグループ一覧内のメンバーシップを確認します。ユーザーのメンバーシップがダイレクト メンバーシップまたは推移性メンバーシップであるグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="d62d4-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="d62d4-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="d62d4-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="d62d4-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d62d4-111">Permissions</span></span>

<span data-ttu-id="d62d4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d62d4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d62d4-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d62d4-114">Permission type</span></span>                        | <span data-ttu-id="d62d4-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d62d4-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d62d4-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d62d4-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d62d4-117">すべてのユーザーとグループがあります。すべての、Directory.accessasuser.all、およびすべてのディレクトリがあります。すべてのユーザーが取得します。すべて、ディレクトリの読み取り。. すべての、ディレクトリは、になります。.</span><span class="sxs-lookup"><span data-stu-id="d62d4-117">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d62d4-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d62d4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d62d4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d62d4-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="d62d4-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d62d4-120">Application</span></span>                            | <span data-ttu-id="d62d4-121">(すべて)、すべてのユーザーを参照します。すべての、またはすべてのディレクトリを取得します。すべてのディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="d62d4-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d62d4-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d62d4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="d62d4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d62d4-123">Request headers</span></span>

| <span data-ttu-id="d62d4-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d62d4-124">Header</span></span>        | <span data-ttu-id="d62d4-125">値</span><span class="sxs-lookup"><span data-stu-id="d62d4-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d62d4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d62d4-126">Authorization</span></span> | <span data-ttu-id="d62d4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d62d4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d62d4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d62d4-129">Content-Type</span></span>  | <span data-ttu-id="d62d4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d62d4-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="d62d4-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="d62d4-131">Request body</span></span>

<span data-ttu-id="d62d4-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="d62d4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d62d4-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="d62d4-133">Parameter</span></span> | <span data-ttu-id="d62d4-134">型</span><span class="sxs-lookup"><span data-stu-id="d62d4-134">Type</span></span>   | <span data-ttu-id="d62d4-135">説明</span><span class="sxs-lookup"><span data-stu-id="d62d4-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="d62d4-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="d62d4-136">groupIds</span></span>  | <span data-ttu-id="d62d4-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d62d4-137">String collection</span></span> | <span data-ttu-id="d62d4-138">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="d62d4-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="d62d4-139">応答</span><span class="sxs-lookup"><span data-stu-id="d62d4-139">Response</span></span>

<span data-ttu-id="d62d4-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d62d4-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d62d4-141">例</span><span class="sxs-lookup"><span data-stu-id="d62d4-141">Example</span></span>

<span data-ttu-id="d62d4-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d62d4-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d62d4-143">要求</span><span class="sxs-lookup"><span data-stu-id="d62d4-143">Request</span></span>

<span data-ttu-id="d62d4-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d62d4-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d62d4-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d62d4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d62d4-146">C#</span><span class="sxs-lookup"><span data-stu-id="d62d4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d62d4-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="d62d4-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d62d4-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="d62d4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d62d4-149">Java</span><span class="sxs-lookup"><span data-stu-id="d62d4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d62d4-150">応答</span><span class="sxs-lookup"><span data-stu-id="d62d4-150">Response</span></span>

<span data-ttu-id="d62d4-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d62d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
