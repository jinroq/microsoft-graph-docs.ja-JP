---
title: checkMemberGroups
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9a19def28bb5747b9a8573c6179e3a2009eca1d0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334970"
---
# <a name="checkmembergroups"></a><span data-ttu-id="71458-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="71458-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71458-p102">指定したグループ一覧内のメンバーシップを確認します。ユーザーのメンバーシップがダイレクト メンバーシップまたは推移性メンバーシップであるグループを一覧から返します。</span><span class="sxs-lookup"><span data-stu-id="71458-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="71458-p103">要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="71458-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="71458-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="71458-111">Permissions</span></span>

<span data-ttu-id="71458-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71458-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71458-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71458-114">Permission type</span></span>                        | <span data-ttu-id="71458-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="71458-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="71458-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71458-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="71458-117">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71458-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="71458-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71458-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71458-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71458-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="71458-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71458-120">Application</span></span>                            | <span data-ttu-id="71458-121">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71458-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="71458-122">**注:** 現在この API には、`Directory.Read.All` 以上のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="71458-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="71458-123">または`User.Read.All` `User.ReadWrite.All`のアクセス許可を使用すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="71458-123">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="71458-124">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="71458-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="71458-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71458-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="71458-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71458-126">Request headers</span></span>

| <span data-ttu-id="71458-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71458-127">Header</span></span>        | <span data-ttu-id="71458-128">値</span><span class="sxs-lookup"><span data-stu-id="71458-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="71458-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="71458-129">Authorization</span></span> | <span data-ttu-id="71458-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="71458-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71458-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71458-132">Content-Type</span></span>  | <span data-ttu-id="71458-133">application/json</span><span class="sxs-lookup"><span data-stu-id="71458-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="71458-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="71458-134">Request body</span></span>

<span data-ttu-id="71458-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="71458-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71458-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="71458-136">Parameter</span></span> | <span data-ttu-id="71458-137">型</span><span class="sxs-lookup"><span data-stu-id="71458-137">Type</span></span>   | <span data-ttu-id="71458-138">説明</span><span class="sxs-lookup"><span data-stu-id="71458-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="71458-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="71458-139">groupIds</span></span>  | <span data-ttu-id="71458-140">String collection</span><span class="sxs-lookup"><span data-stu-id="71458-140">String collection</span></span> | <span data-ttu-id="71458-141">グループ ID の配列</span><span class="sxs-lookup"><span data-stu-id="71458-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="71458-142">応答</span><span class="sxs-lookup"><span data-stu-id="71458-142">Response</span></span>

<span data-ttu-id="71458-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="71458-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71458-144">例</span><span class="sxs-lookup"><span data-stu-id="71458-144">Example</span></span>

<span data-ttu-id="71458-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="71458-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="71458-146">要求</span><span class="sxs-lookup"><span data-stu-id="71458-146">Request</span></span>

<span data-ttu-id="71458-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71458-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="71458-148">応答</span><span class="sxs-lookup"><span data-stu-id="71458-148">Response</span></span>

<span data-ttu-id="71458-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71458-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
