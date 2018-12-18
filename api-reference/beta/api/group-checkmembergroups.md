---
title: 'グループ: checkMemberGroups'
description: グループの指定されたリスト内のメンバーシップを確認します。 リストから先のグループを返します。
author: dkershaw10
ms.openlocfilehash: 0868f8ed2b0b1bb1afaeb8741a8e7156608c6388
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348028"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="0edd5-104">グループ: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="0edd5-104">group: checkMemberGroups</span></span>

> <span data-ttu-id="0edd5-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0edd5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0edd5-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0edd5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0edd5-p103">指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="0edd5-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="0edd5-p104">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="0edd5-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="0edd5-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0edd5-113">Permissions</span></span>

<span data-ttu-id="0edd5-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0edd5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0edd5-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0edd5-116">Permission type</span></span>                        | <span data-ttu-id="0edd5-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0edd5-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="0edd5-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0edd5-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="0edd5-119">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0edd5-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="0edd5-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0edd5-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0edd5-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0edd5-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="0edd5-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0edd5-122">Application</span></span>                            | <span data-ttu-id="0edd5-123">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0edd5-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="0edd5-124">**注:** この API は現在必要があります、`Directory.Read.All`アクセス権またはそれ以上です。</span><span class="sxs-lookup"><span data-stu-id="0edd5-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="0edd5-125">使用して、`Group.Read.All`のアクセス許可エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="0edd5-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="0edd5-126">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="0edd5-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="0edd5-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0edd5-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="0edd5-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0edd5-128">Request headers</span></span>

| <span data-ttu-id="0edd5-129">名前</span><span class="sxs-lookup"><span data-stu-id="0edd5-129">Name</span></span>          | <span data-ttu-id="0edd5-130">種類</span><span class="sxs-lookup"><span data-stu-id="0edd5-130">Type</span></span>   | <span data-ttu-id="0edd5-131">説明</span><span class="sxs-lookup"><span data-stu-id="0edd5-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="0edd5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="0edd5-132">Authorization</span></span> | <span data-ttu-id="0edd5-133">string</span><span class="sxs-lookup"><span data-stu-id="0edd5-133">string</span></span> | <span data-ttu-id="0edd5-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0edd5-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0edd5-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="0edd5-136">Request body</span></span>

<span data-ttu-id="0edd5-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0edd5-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0edd5-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0edd5-138">Parameter</span></span> | <span data-ttu-id="0edd5-139">種類</span><span class="sxs-lookup"><span data-stu-id="0edd5-139">Type</span></span>   | <span data-ttu-id="0edd5-140">説明</span><span class="sxs-lookup"><span data-stu-id="0edd5-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="0edd5-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="0edd5-141">groupIds</span></span>  | <span data-ttu-id="0edd5-142">String</span><span class="sxs-lookup"><span data-stu-id="0edd5-142">String</span></span> | <span data-ttu-id="0edd5-143">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="0edd5-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="0edd5-144">応答</span><span class="sxs-lookup"><span data-stu-id="0edd5-144">Response</span></span>

<span data-ttu-id="0edd5-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0edd5-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0edd5-146">例</span><span class="sxs-lookup"><span data-stu-id="0edd5-146">Example</span></span>

<span data-ttu-id="0edd5-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0edd5-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="0edd5-148">要求</span><span class="sxs-lookup"><span data-stu-id="0edd5-148">Request</span></span>

<span data-ttu-id="0edd5-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0edd5-149">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="0edd5-150">応答</span><span class="sxs-lookup"><span data-stu-id="0edd5-150">Response</span></span>

<span data-ttu-id="0edd5-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0edd5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
