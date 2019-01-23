---
title: 'user: getMemberGroups'
description: ユーザーがのメンバーであるすべてのグループを返します。 チェックは推移機能が、読み取りとは異なり、
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb6a10a80503d8842442e2678bcf52ee6154e3f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424211"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="67f4e-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="67f4e-104">user: getMemberGroups</span></span>

> <span data-ttu-id="67f4e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67f4e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67f4e-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67f4e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67f4e-p103">ユーザーがメンバーであるすべてのグループを返します。チェックは推移的であり、ユーザーが直接メンバーであるグループのみを返す [memberOf](../api/user-list-memberof.md) ナビゲーション プロパティの読み取りとは異なります。</span><span class="sxs-lookup"><span data-stu-id="67f4e-p103">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="67f4e-p104">この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。各要求を返すことができるグループの最大数は 2046 です。Office 365 グループにグループを含めることはできません。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。</span><span class="sxs-lookup"><span data-stu-id="67f4e-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f4e-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="67f4e-113">Permissions</span></span>

<span data-ttu-id="67f4e-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67f4e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67f4e-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67f4e-116">Permission type</span></span>                        | <span data-ttu-id="67f4e-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="67f4e-117">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="67f4e-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67f4e-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="67f4e-119">User.Read、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67f4e-119">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="67f4e-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67f4e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f4e-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67f4e-121">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="67f4e-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67f4e-122">Application</span></span>                            | <span data-ttu-id="67f4e-123">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67f4e-123">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

> <span data-ttu-id="67f4e-124">**注:** この API は現在必要があります、`Directory.Read.All`アクセス権またはそれ以上です。</span><span class="sxs-lookup"><span data-stu-id="67f4e-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="67f4e-125">単独または組み合わせて、Group.Read.All のアクセス許可を使用して、`User.`のアクセス許可エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="67f4e-125">Using the Group.Read.All permission, either alone or in combination with a `User.` permission, will return an error.</span></span> <span data-ttu-id="67f4e-126">これは既知のバグです。</span><span class="sxs-lookup"><span data-stu-id="67f4e-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="67f4e-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67f4e-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="67f4e-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67f4e-128">Request headers</span></span>

| <span data-ttu-id="67f4e-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67f4e-129">Header</span></span>        | <span data-ttu-id="67f4e-130">値</span><span class="sxs-lookup"><span data-stu-id="67f4e-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="67f4e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="67f4e-131">Authorization</span></span> | <span data-ttu-id="67f4e-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="67f4e-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67f4e-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67f4e-134">Content-Type</span></span>  | <span data-ttu-id="67f4e-135">application/json</span><span class="sxs-lookup"><span data-stu-id="67f4e-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="67f4e-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="67f4e-136">Request body</span></span>

<span data-ttu-id="67f4e-137">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="67f4e-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="67f4e-138">パラメーター</span><span class="sxs-lookup"><span data-stu-id="67f4e-138">Parameter</span></span>           | <span data-ttu-id="67f4e-139">Type</span><span class="sxs-lookup"><span data-stu-id="67f4e-139">Type</span></span>    | <span data-ttu-id="67f4e-140">説明</span><span class="sxs-lookup"><span data-stu-id="67f4e-140">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="67f4e-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="67f4e-141">securityEnabledOnly</span></span> | <span data-ttu-id="67f4e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="67f4e-142">Boolean</span></span> | <span data-ttu-id="67f4e-p108">ユーザーがメンバーであるセキュリティ グループのみを返すように指定するには **true**、ユーザーがメンバーであるすべてのグループとディレクトリ ロールを返すように指定するには **false** を設定します。注:このパラメーターの **true** 設定は、ユーザーに対してこのメソッドを呼び出したときにのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="67f4e-p108">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="67f4e-145">応答</span><span class="sxs-lookup"><span data-stu-id="67f4e-145">Response</span></span>

<span data-ttu-id="67f4e-146">成功した場合、このメソッドはユーザーがメンバーであるグループの ID を含んだ応答本文で `200 OK` 応答コードと文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="67f4e-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="67f4e-147">例</span><span class="sxs-lookup"><span data-stu-id="67f4e-147">Example</span></span>

<span data-ttu-id="67f4e-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="67f4e-148">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="67f4e-149">要求</span><span class="sxs-lookup"><span data-stu-id="67f4e-149">Request</span></span>

<span data-ttu-id="67f4e-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67f4e-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="67f4e-151">応答</span><span class="sxs-lookup"><span data-stu-id="67f4e-151">Response</span></span>

<span data-ttu-id="67f4e-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67f4e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
