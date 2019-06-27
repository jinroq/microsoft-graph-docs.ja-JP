---
title: 'user: getMemberGroups'
description: ユーザーがメンバーであるすべてのグループを返します。 次の読み取りとは異なり、チェックは推移的です。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a99aca467e34d82025a45d5a898235f5cc7bf368
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277981"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="c2a79-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="c2a79-104">user: getMemberGroups</span></span>

<span data-ttu-id="c2a79-p102">ユーザーがメンバーであるすべてのグループを返します。チェックは推移的であり、ユーザーが直接メンバーであるグループのみを返す [memberOf](../api/user-list-memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="c2a79-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="c2a79-p103">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="c2a79-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2a79-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2a79-111">Permissions</span></span>

<span data-ttu-id="c2a79-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2a79-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2a79-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2a79-114">Permission type</span></span>                        | <span data-ttu-id="c2a79-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2a79-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c2a79-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2a79-116">Delegated (work or school account)</span></span>     |  <span data-ttu-id="c2a79-117">User.Read、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2a79-117">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="c2a79-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2a79-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2a79-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2a79-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="c2a79-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2a79-120">Application</span></span>                            | <span data-ttu-id="c2a79-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a79-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

## <a name="http-request"></a><span data-ttu-id="c2a79-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2a79-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="c2a79-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2a79-123">Request headers</span></span>

| <span data-ttu-id="c2a79-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2a79-124">Header</span></span>        | <span data-ttu-id="c2a79-125">値</span><span class="sxs-lookup"><span data-stu-id="c2a79-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c2a79-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2a79-126">Authorization</span></span> | <span data-ttu-id="c2a79-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c2a79-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2a79-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2a79-129">Content-Type</span></span>  | <span data-ttu-id="c2a79-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c2a79-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="c2a79-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2a79-131">Request body</span></span>

<span data-ttu-id="c2a79-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c2a79-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c2a79-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c2a79-133">Parameter</span></span>           | <span data-ttu-id="c2a79-134">型</span><span class="sxs-lookup"><span data-stu-id="c2a79-134">Type</span></span>    | <span data-ttu-id="c2a79-135">説明</span><span class="sxs-lookup"><span data-stu-id="c2a79-135">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c2a79-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c2a79-136">securityEnabledOnly</span></span> | <span data-ttu-id="c2a79-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2a79-137">Boolean</span></span> | <span data-ttu-id="c2a79-p106">ユーザーがメンバーであるセキュリティ グループのみを返すように指定するには **true**、ユーザーがメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。注:このパラメーターの **true** 設定は、ユーザーに対してこのメソッドを呼び出したときにのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c2a79-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="c2a79-140">応答</span><span class="sxs-lookup"><span data-stu-id="c2a79-140">Response</span></span>

<span data-ttu-id="c2a79-141">成功した場合、このメソッドはユーザーがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c2a79-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="c2a79-142">例</span><span class="sxs-lookup"><span data-stu-id="c2a79-142">Example</span></span>

<span data-ttu-id="c2a79-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c2a79-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c2a79-144">要求</span><span class="sxs-lookup"><span data-stu-id="c2a79-144">Request</span></span>

<span data-ttu-id="c2a79-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2a79-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="c2a79-146">応答</span><span class="sxs-lookup"><span data-stu-id="c2a79-146">Response</span></span>

<span data-ttu-id="c2a79-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2a79-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2a79-150">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="c2a79-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2a79-151">C#</span><span class="sxs-lookup"><span data-stu-id="c2a79-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2a79-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2a79-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_getmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2a79-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2a79-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_getmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
