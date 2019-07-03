---
title: checkMemberGroups
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 272b377534bd9fbee676135240d85983bf0f121b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460561"
---
# <a name="checkmembergroups"></a><span data-ttu-id="9c58e-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9c58e-104">checkMemberGroups</span></span>

<span data-ttu-id="9c58e-p102">指定したグループ一覧内のメンバーシップを確認します。ユーザーのメンバーシップがダイレクト メンバーシップまたは推移性メンバーシップであるグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="9c58e-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="9c58e-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="9c58e-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c58e-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9c58e-111">Permissions</span></span>

<span data-ttu-id="9c58e-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c58e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c58e-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c58e-114">Permission type</span></span>                        | <span data-ttu-id="9c58e-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c58e-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9c58e-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c58e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c58e-117">User.ReadBasic.All および Group.Read.All、User.Read.All および Group.Read.All、User.ReadWrite.All および Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c58e-117">User.Read and Group.Read.All, User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9c58e-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c58e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c58e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c58e-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="9c58e-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c58e-120">Application</span></span>                            | <span data-ttu-id="9c58e-121">User.Read.All および Group.Read.All、User.ReadWrite.All および Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c58e-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c58e-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c58e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9c58e-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c58e-123">Request headers</span></span>

| <span data-ttu-id="9c58e-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c58e-124">Header</span></span>        | <span data-ttu-id="9c58e-125">値</span><span class="sxs-lookup"><span data-stu-id="9c58e-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9c58e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c58e-126">Authorization</span></span> | <span data-ttu-id="9c58e-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9c58e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c58e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c58e-129">Content-Type</span></span>  | <span data-ttu-id="9c58e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9c58e-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9c58e-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c58e-131">Request body</span></span>

<span data-ttu-id="9c58e-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="9c58e-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9c58e-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9c58e-133">Parameter</span></span> | <span data-ttu-id="9c58e-134">型</span><span class="sxs-lookup"><span data-stu-id="9c58e-134">Type</span></span>              | <span data-ttu-id="9c58e-135">説明</span><span class="sxs-lookup"><span data-stu-id="9c58e-135">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="9c58e-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="9c58e-136">groupIds</span></span>  | <span data-ttu-id="9c58e-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9c58e-137">String collection</span></span> | <span data-ttu-id="9c58e-138">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="9c58e-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="9c58e-139">応答</span><span class="sxs-lookup"><span data-stu-id="9c58e-139">Response</span></span>

<span data-ttu-id="9c58e-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9c58e-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c58e-141">例</span><span class="sxs-lookup"><span data-stu-id="9c58e-141">Example</span></span>

<span data-ttu-id="9c58e-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9c58e-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9c58e-143">要求</span><span class="sxs-lookup"><span data-stu-id="9c58e-143">Request</span></span>

<span data-ttu-id="9c58e-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9c58e-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9c58e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c58e-145">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c58e-146">C#</span><span class="sxs-lookup"><span data-stu-id="9c58e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c58e-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c58e-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c58e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c58e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9c58e-149">応答</span><span class="sxs-lookup"><span data-stu-id="9c58e-149">Response</span></span>

<span data-ttu-id="9c58e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9c58e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
