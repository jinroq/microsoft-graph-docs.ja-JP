---
title: 'グループ: getMemberGroups'
description: 指定されたグループがメンバーであるすべてのグループを返します。 チェックは、グループが直接メンバーであるグループのみを返す memberOf ナビゲーション プロパティの読み取りとは異なり、推移的です。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b37ac8f14284de25c95862800a692ca52e29e216
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337364"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="b6e1d-104">グループ: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b6e1d-104">group: getMemberGroups</span></span>

<span data-ttu-id="b6e1d-p102">指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す [memberOf](../api/group-list-memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="b6e1d-p103">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6e1d-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6e1d-111">Permissions</span></span>

<span data-ttu-id="b6e1d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6e1d-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6e1d-114">Permission type</span></span>                        | <span data-ttu-id="b6e1d-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6e1d-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b6e1d-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6e1d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6e1d-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6e1d-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b6e1d-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6e1d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6e1d-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="b6e1d-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6e1d-120">Application</span></span>                            | <span data-ttu-id="b6e1d-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e1d-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |


## <a name="http-request"></a><span data-ttu-id="b6e1d-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6e1d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="b6e1d-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6e1d-123">Request headers</span></span>

| <span data-ttu-id="b6e1d-124">名前</span><span class="sxs-lookup"><span data-stu-id="b6e1d-124">Name</span></span>          | <span data-ttu-id="b6e1d-125">種類</span><span class="sxs-lookup"><span data-stu-id="b6e1d-125">Type</span></span>   | <span data-ttu-id="b6e1d-126">説明</span><span class="sxs-lookup"><span data-stu-id="b6e1d-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="b6e1d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6e1d-127">Authorization</span></span> | <span data-ttu-id="b6e1d-128">string</span><span class="sxs-lookup"><span data-stu-id="b6e1d-128">string</span></span> | <span data-ttu-id="b6e1d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6e1d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6e1d-131">Request body</span></span>

<span data-ttu-id="b6e1d-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b6e1d-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b6e1d-133">Parameter</span></span>           | <span data-ttu-id="b6e1d-134">型</span><span class="sxs-lookup"><span data-stu-id="b6e1d-134">Type</span></span>    | <span data-ttu-id="b6e1d-135">説明</span><span class="sxs-lookup"><span data-stu-id="b6e1d-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="b6e1d-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b6e1d-136">securityEnabledOnly</span></span> | <span data-ttu-id="b6e1d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6e1d-137">Boolean</span></span> | <span data-ttu-id="b6e1d-p106">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="b6e1d-140">応答</span><span class="sxs-lookup"><span data-stu-id="b6e1d-140">Response</span></span>

<span data-ttu-id="b6e1d-141">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="b6e1d-142">例</span><span class="sxs-lookup"><span data-stu-id="b6e1d-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b6e1d-143">要求</span><span class="sxs-lookup"><span data-stu-id="b6e1d-143">Request</span></span>

<span data-ttu-id="b6e1d-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b6e1d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6e1d-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b6e1d-146">C#</span><span class="sxs-lookup"><span data-stu-id="b6e1d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6e1d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6e1d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b6e1d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6e1d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b6e1d-149">Java</span><span class="sxs-lookup"><span data-stu-id="b6e1d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6e1d-150">応答</span><span class="sxs-lookup"><span data-stu-id="b6e1d-150">Response</span></span>

<span data-ttu-id="b6e1d-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-151">The following is an example of the response.</span></span>

> <span data-ttu-id="b6e1d-152">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6e1d-153">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b6e1d-153">All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
