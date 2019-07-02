---
title: checkMemberGroups
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 171dffcb912c2ac26ecc3cd01388299228ca44db
ms.sourcegitcommit: 6d8bf390380b9434ba626d6dc5101afcf6ba6f8b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2019
ms.locfileid: "35395164"
---
# <a name="checkmembergroups"></a><span data-ttu-id="52f73-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="52f73-104">checkMemberGroups</span></span>

<span data-ttu-id="52f73-p102">指定したグループ一覧内のメンバーシップを確認します。ユーザーのメンバーシップがダイレクト メンバーシップまたは推移性メンバーシップであるグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="52f73-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="52f73-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="52f73-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f73-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52f73-111">Permissions</span></span>

<span data-ttu-id="52f73-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52f73-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52f73-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52f73-114">Permission type</span></span>                        | <span data-ttu-id="52f73-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52f73-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="52f73-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52f73-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="52f73-117">User.ReadBasic.All および Group.Read.All、User.Read.All および Group.Read.All、User.ReadWrite.All および Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="52f73-117">User.Read and Group.Read.All, User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="52f73-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52f73-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52f73-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52f73-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="52f73-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52f73-120">Application</span></span>                            | <span data-ttu-id="52f73-121">User.Read.All および Group.Read.All、User.ReadWrite.All および Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f73-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52f73-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52f73-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="52f73-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52f73-123">Request headers</span></span>

| <span data-ttu-id="52f73-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52f73-124">Header</span></span>        | <span data-ttu-id="52f73-125">値</span><span class="sxs-lookup"><span data-stu-id="52f73-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="52f73-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="52f73-126">Authorization</span></span> | <span data-ttu-id="52f73-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52f73-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52f73-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52f73-129">Content-Type</span></span>  | <span data-ttu-id="52f73-130">application/json</span><span class="sxs-lookup"><span data-stu-id="52f73-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="52f73-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="52f73-131">Request body</span></span>

<span data-ttu-id="52f73-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="52f73-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52f73-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="52f73-133">Parameter</span></span> | <span data-ttu-id="52f73-134">型</span><span class="sxs-lookup"><span data-stu-id="52f73-134">Type</span></span>              | <span data-ttu-id="52f73-135">説明</span><span class="sxs-lookup"><span data-stu-id="52f73-135">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="52f73-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="52f73-136">groupIds</span></span>  | <span data-ttu-id="52f73-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="52f73-137">String collection</span></span> | <span data-ttu-id="52f73-138">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="52f73-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="52f73-139">応答</span><span class="sxs-lookup"><span data-stu-id="52f73-139">Response</span></span>

<span data-ttu-id="52f73-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52f73-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52f73-141">例</span><span class="sxs-lookup"><span data-stu-id="52f73-141">Example</span></span>

<span data-ttu-id="52f73-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="52f73-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="52f73-143">要求</span><span class="sxs-lookup"><span data-stu-id="52f73-143">Request</span></span>

<span data-ttu-id="52f73-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52f73-144">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="52f73-145">応答</span><span class="sxs-lookup"><span data-stu-id="52f73-145">Response</span></span>

<span data-ttu-id="52f73-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52f73-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="52f73-149">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="52f73-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52f73-150">C#</span><span class="sxs-lookup"><span data-stu-id="52f73-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52f73-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="52f73-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52f73-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f73-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
