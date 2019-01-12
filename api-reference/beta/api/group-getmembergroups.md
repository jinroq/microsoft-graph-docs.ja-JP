---
title: 'グループ: getMemberGroups'
description: 指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す memberOf ナビゲーション プロパティの読み取りとは異なります。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e485c80a06fc2d124dec728ab3ffcdfb8dcce105
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921536"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="ca2e1-104">グループ: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ca2e1-104">group: getMemberGroups</span></span>

> <span data-ttu-id="ca2e1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca2e1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca2e1-p103">指定されたグループがメンバーであるすべてのグループを返します。チェックは推移的であり、グループが直接メンバーであるグループのみを返す [memberOf](../api/group-list-memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p103">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="ca2e1-p104">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca2e1-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca2e1-113">Permissions</span></span>

<span data-ttu-id="ca2e1-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca2e1-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca2e1-116">Permission type</span></span>                        | <span data-ttu-id="ca2e1-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca2e1-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="ca2e1-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca2e1-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca2e1-119">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca2e1-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ca2e1-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca2e1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca2e1-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="ca2e1-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca2e1-122">Application</span></span>                            | <span data-ttu-id="ca2e1-123">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca2e1-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="ca2e1-124">**注:** この API は現在必要があります、`Directory.Read.All`アクセス権またはそれ以上です。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="ca2e1-125">使用して、`Group.Read.All`のアクセス許可エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="ca2e1-126">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca2e1-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca2e1-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="ca2e1-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca2e1-128">Request headers</span></span>

| <span data-ttu-id="ca2e1-129">名前</span><span class="sxs-lookup"><span data-stu-id="ca2e1-129">Name</span></span>          | <span data-ttu-id="ca2e1-130">型</span><span class="sxs-lookup"><span data-stu-id="ca2e1-130">Type</span></span>   | <span data-ttu-id="ca2e1-131">説明</span><span class="sxs-lookup"><span data-stu-id="ca2e1-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="ca2e1-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca2e1-132">Authorization</span></span> | <span data-ttu-id="ca2e1-133">string</span><span class="sxs-lookup"><span data-stu-id="ca2e1-133">string</span></span> | <span data-ttu-id="ca2e1-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca2e1-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca2e1-136">Request body</span></span>

<span data-ttu-id="ca2e1-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca2e1-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca2e1-138">Parameter</span></span>           | <span data-ttu-id="ca2e1-139">型</span><span class="sxs-lookup"><span data-stu-id="ca2e1-139">Type</span></span>    | <span data-ttu-id="ca2e1-140">説明</span><span class="sxs-lookup"><span data-stu-id="ca2e1-140">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="ca2e1-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ca2e1-141">securityEnabledOnly</span></span> | <span data-ttu-id="ca2e1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca2e1-142">Boolean</span></span> | <span data-ttu-id="ca2e1-p108">**false** に設定します。セキュリティが有効なグループのみを返すことは、ユーザーに対してのみサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p108">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="ca2e1-145">応答</span><span class="sxs-lookup"><span data-stu-id="ca2e1-145">Response</span></span>

<span data-ttu-id="ca2e1-146">成功した場合、このメソッドはグループがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="ca2e1-147">例</span><span class="sxs-lookup"><span data-stu-id="ca2e1-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ca2e1-148">要求</span><span class="sxs-lookup"><span data-stu-id="ca2e1-148">Request</span></span>

<span data-ttu-id="ca2e1-149">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-149">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="ca2e1-150">応答</span><span class="sxs-lookup"><span data-stu-id="ca2e1-150">Response</span></span>

<span data-ttu-id="ca2e1-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-151">The following is an example of the response.</span></span>

> <span data-ttu-id="ca2e1-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
