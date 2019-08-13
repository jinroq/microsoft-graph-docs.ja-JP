---
title: 'グループ: checkMemberGroups'
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 90c524ecb447b6020e350ae7c8879c939d2421cd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337560"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="08763-104">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="08763-104">group: checkMemberGroups</span></span>

<span data-ttu-id="08763-p102">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="08763-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="08763-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="08763-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="08763-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08763-111">Permissions</span></span>

<span data-ttu-id="08763-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08763-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08763-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08763-114">Permission type</span></span>                        | <span data-ttu-id="08763-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08763-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="08763-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08763-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="08763-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08763-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="08763-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08763-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08763-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08763-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="08763-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08763-120">Application</span></span>                            | <span data-ttu-id="08763-121">Group.Read.All、Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="08763-121">Group.Read.All, Directory.Read.All.</span></span> <span data-ttu-id="08763-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08763-122">Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="08763-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08763-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="08763-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08763-124">Request headers</span></span>

| <span data-ttu-id="08763-125">名前</span><span class="sxs-lookup"><span data-stu-id="08763-125">Name</span></span>          | <span data-ttu-id="08763-126">種類</span><span class="sxs-lookup"><span data-stu-id="08763-126">Type</span></span>   | <span data-ttu-id="08763-127">説明</span><span class="sxs-lookup"><span data-stu-id="08763-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="08763-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="08763-128">Authorization</span></span> | <span data-ttu-id="08763-129">string</span><span class="sxs-lookup"><span data-stu-id="08763-129">string</span></span> | <span data-ttu-id="08763-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08763-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08763-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="08763-132">Request body</span></span>

<span data-ttu-id="08763-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="08763-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08763-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="08763-134">Parameter</span></span> | <span data-ttu-id="08763-135">型</span><span class="sxs-lookup"><span data-stu-id="08763-135">Type</span></span>              | <span data-ttu-id="08763-136">説明</span><span class="sxs-lookup"><span data-stu-id="08763-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="08763-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="08763-137">groupIds</span></span>  | <span data-ttu-id="08763-138">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="08763-138">String collection</span></span> | <span data-ttu-id="08763-139">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="08763-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="08763-140">応答</span><span class="sxs-lookup"><span data-stu-id="08763-140">Response</span></span>

<span data-ttu-id="08763-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08763-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08763-142">例</span><span class="sxs-lookup"><span data-stu-id="08763-142">Example</span></span>

<span data-ttu-id="08763-143">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="08763-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="08763-144">要求</span><span class="sxs-lookup"><span data-stu-id="08763-144">Request</span></span>

<span data-ttu-id="08763-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08763-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="08763-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="08763-146">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08763-147">C#</span><span class="sxs-lookup"><span data-stu-id="08763-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08763-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08763-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08763-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08763-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08763-150">Java</span><span class="sxs-lookup"><span data-stu-id="08763-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08763-151">応答</span><span class="sxs-lookup"><span data-stu-id="08763-151">Response</span></span>

<span data-ttu-id="08763-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08763-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
