---
title: 'グループ: checkMemberGroups'
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: af5aa9b1d291508530eaba72892e657ce95a627e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954041"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="191d7-104">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="191d7-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="191d7-p102">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="191d7-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="191d7-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="191d7-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="191d7-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="191d7-111">Permissions</span></span>

<span data-ttu-id="191d7-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="191d7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="191d7-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="191d7-114">Permission type</span></span>                        | <span data-ttu-id="191d7-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="191d7-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="191d7-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="191d7-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="191d7-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="191d7-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="191d7-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="191d7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="191d7-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="191d7-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="191d7-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="191d7-120">Application</span></span>                            | <span data-ttu-id="191d7-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="191d7-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="191d7-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="191d7-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="191d7-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="191d7-123">Request headers</span></span>

| <span data-ttu-id="191d7-124">名前</span><span class="sxs-lookup"><span data-stu-id="191d7-124">Name</span></span>          | <span data-ttu-id="191d7-125">型</span><span class="sxs-lookup"><span data-stu-id="191d7-125">Type</span></span>   | <span data-ttu-id="191d7-126">説明</span><span class="sxs-lookup"><span data-stu-id="191d7-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="191d7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="191d7-127">Authorization</span></span> | <span data-ttu-id="191d7-128">string</span><span class="sxs-lookup"><span data-stu-id="191d7-128">string</span></span> | <span data-ttu-id="191d7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="191d7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="191d7-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="191d7-131">Request body</span></span>

<span data-ttu-id="191d7-132">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="191d7-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="191d7-133">パラメーター</span><span class="sxs-lookup"><span data-stu-id="191d7-133">Parameter</span></span> | <span data-ttu-id="191d7-134">型</span><span class="sxs-lookup"><span data-stu-id="191d7-134">Type</span></span>   | <span data-ttu-id="191d7-135">説明</span><span class="sxs-lookup"><span data-stu-id="191d7-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="191d7-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="191d7-136">groupIds</span></span>  | <span data-ttu-id="191d7-137">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="191d7-137">String collection</span></span> | <span data-ttu-id="191d7-138">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="191d7-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="191d7-139">応答</span><span class="sxs-lookup"><span data-stu-id="191d7-139">Response</span></span>

<span data-ttu-id="191d7-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="191d7-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="191d7-141">例</span><span class="sxs-lookup"><span data-stu-id="191d7-141">Example</span></span>

<span data-ttu-id="191d7-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="191d7-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="191d7-143">要求</span><span class="sxs-lookup"><span data-stu-id="191d7-143">Request</span></span>

<span data-ttu-id="191d7-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="191d7-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="191d7-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="191d7-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="191d7-146">C#</span><span class="sxs-lookup"><span data-stu-id="191d7-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="191d7-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="191d7-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="191d7-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="191d7-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="191d7-149">Java</span><span class="sxs-lookup"><span data-stu-id="191d7-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="191d7-150">応答</span><span class="sxs-lookup"><span data-stu-id="191d7-150">Response</span></span>

<span data-ttu-id="191d7-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="191d7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
