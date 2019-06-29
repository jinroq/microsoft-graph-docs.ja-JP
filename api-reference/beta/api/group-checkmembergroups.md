---
title: 'グループ: checkMemberGroups'
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 524cfeff7a01de50d33224089557ecd62081dc77
ms.sourcegitcommit: 6d8bf390380b9434ba626d6dc5101afcf6ba6f8b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2019
ms.locfileid: "35395150"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="b1868-104">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b1868-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1868-p102">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="b1868-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="b1868-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="b1868-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1868-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b1868-111">Permissions</span></span>

<span data-ttu-id="b1868-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1868-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1868-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1868-114">Permission type</span></span>                        | <span data-ttu-id="b1868-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1868-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b1868-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1868-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1868-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1868-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b1868-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1868-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1868-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1868-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="b1868-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1868-120">Application</span></span>                            | <span data-ttu-id="b1868-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1868-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="b1868-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1868-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="b1868-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1868-123">Request headers</span></span>

| <span data-ttu-id="b1868-124">名前</span><span class="sxs-lookup"><span data-stu-id="b1868-124">Name</span></span>          | <span data-ttu-id="b1868-125">型</span><span class="sxs-lookup"><span data-stu-id="b1868-125">Type</span></span>   | <span data-ttu-id="b1868-126">説明</span><span class="sxs-lookup"><span data-stu-id="b1868-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="b1868-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1868-127">Authorization</span></span> | <span data-ttu-id="b1868-128">string</span><span class="sxs-lookup"><span data-stu-id="b1868-128">string</span></span> | <span data-ttu-id="b1868-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b1868-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1868-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1868-131">Request body</span></span>

<span data-ttu-id="b1868-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b1868-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1868-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b1868-133">Parameter</span></span> | <span data-ttu-id="b1868-134">型</span><span class="sxs-lookup"><span data-stu-id="b1868-134">Type</span></span>   | <span data-ttu-id="b1868-135">説明</span><span class="sxs-lookup"><span data-stu-id="b1868-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="b1868-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="b1868-136">groupIds</span></span>  | <span data-ttu-id="b1868-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b1868-137">String collection</span></span> | <span data-ttu-id="b1868-138">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="b1868-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="b1868-139">応答</span><span class="sxs-lookup"><span data-stu-id="b1868-139">Response</span></span>

<span data-ttu-id="b1868-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b1868-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1868-141">例</span><span class="sxs-lookup"><span data-stu-id="b1868-141">Example</span></span>

<span data-ttu-id="b1868-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b1868-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b1868-143">要求</span><span class="sxs-lookup"><span data-stu-id="b1868-143">Request</span></span>

<span data-ttu-id="b1868-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1868-144">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="b1868-145">応答</span><span class="sxs-lookup"><span data-stu-id="b1868-145">Response</span></span>

<span data-ttu-id="b1868-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1868-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b1868-149">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b1868-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b1868-150">C#</span><span class="sxs-lookup"><span data-stu-id="b1868-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1868-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1868-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b1868-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="b1868-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
