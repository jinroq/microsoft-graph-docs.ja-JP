---
title: 'グループ: getMemberGroups'
description: 指定されたグループがメンバーであるすべてのグループを返します。 チェックは、グループが直接メンバーであるグループのみを返す memberOf ナビゲーション プロパティの読み取りとは異なり、推移的です。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e5b1d23ebce82770e218af0a3b4758b9ff86b07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953858"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="791ed-104">グループ: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="791ed-104">group: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="791ed-p102">指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す [memberOf](../api/group-list-memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="791ed-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="791ed-p103">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="791ed-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="791ed-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="791ed-111">Permissions</span></span>

<span data-ttu-id="791ed-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="791ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="791ed-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="791ed-114">Permission type</span></span>                        | <span data-ttu-id="791ed-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="791ed-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="791ed-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="791ed-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="791ed-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="791ed-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="791ed-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="791ed-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791ed-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="791ed-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="791ed-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="791ed-120">Application</span></span>                            | <span data-ttu-id="791ed-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ed-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="791ed-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="791ed-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="791ed-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="791ed-123">Request headers</span></span>

| <span data-ttu-id="791ed-124">名前</span><span class="sxs-lookup"><span data-stu-id="791ed-124">Name</span></span>          | <span data-ttu-id="791ed-125">型</span><span class="sxs-lookup"><span data-stu-id="791ed-125">Type</span></span>   | <span data-ttu-id="791ed-126">説明</span><span class="sxs-lookup"><span data-stu-id="791ed-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="791ed-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="791ed-127">Authorization</span></span> | <span data-ttu-id="791ed-128">string</span><span class="sxs-lookup"><span data-stu-id="791ed-128">string</span></span> | <span data-ttu-id="791ed-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="791ed-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="791ed-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="791ed-131">Request body</span></span>

<span data-ttu-id="791ed-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="791ed-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="791ed-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="791ed-133">Parameter</span></span>           | <span data-ttu-id="791ed-134">型</span><span class="sxs-lookup"><span data-stu-id="791ed-134">Type</span></span>    | <span data-ttu-id="791ed-135">説明</span><span class="sxs-lookup"><span data-stu-id="791ed-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="791ed-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="791ed-136">securityEnabledOnly</span></span> | <span data-ttu-id="791ed-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ed-137">Boolean</span></span> | <span data-ttu-id="791ed-p106">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="791ed-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="791ed-140">応答</span><span class="sxs-lookup"><span data-stu-id="791ed-140">Response</span></span>

<span data-ttu-id="791ed-141">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="791ed-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="791ed-142">例</span><span class="sxs-lookup"><span data-stu-id="791ed-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="791ed-143">要求</span><span class="sxs-lookup"><span data-stu-id="791ed-143">Request</span></span>

<span data-ttu-id="791ed-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="791ed-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="791ed-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="791ed-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="791ed-146">C#</span><span class="sxs-lookup"><span data-stu-id="791ed-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="791ed-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="791ed-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="791ed-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="791ed-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="791ed-149">Java</span><span class="sxs-lookup"><span data-stu-id="791ed-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="791ed-150">応答</span><span class="sxs-lookup"><span data-stu-id="791ed-150">Response</span></span>

<span data-ttu-id="791ed-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="791ed-151">The following is an example of the response.</span></span>

> <span data-ttu-id="791ed-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="791ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
