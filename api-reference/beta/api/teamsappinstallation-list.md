---
title: チームのアプリを一覧表示する
description: 指定したチームにインストールされているアプリのリストを取得します。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a02a94b19f431a37b75e23f8106c0fac9aa7f43a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409358"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="221fe-103">チームのアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="221fe-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="221fe-104">指定した[チーム](../resources/team.md)に[インストールされているアプリ](../resources/teamsappinstallation.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="221fe-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="221fe-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="221fe-105">Permissions</span></span>

<span data-ttu-id="221fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="221fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="221fe-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="221fe-108">Permission type</span></span>      | <span data-ttu-id="221fe-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="221fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="221fe-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="221fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="221fe-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="221fe-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="221fe-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="221fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="221fe-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="221fe-113">Not supported.</span></span>    |
|<span data-ttu-id="221fe-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="221fe-114">Application</span></span> | <span data-ttu-id="221fe-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="221fe-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="221fe-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="221fe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="221fe-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="221fe-117">Optional query parameters</span></span>

<span data-ttu-id="221fe-118">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="221fe-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="221fe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="221fe-119">Request headers</span></span>

| <span data-ttu-id="221fe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="221fe-120">Header</span></span>       | <span data-ttu-id="221fe-121">値</span><span class="sxs-lookup"><span data-stu-id="221fe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="221fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="221fe-122">Authorization</span></span>  | <span data-ttu-id="221fe-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="221fe-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="221fe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="221fe-125">Request body</span></span>

<span data-ttu-id="221fe-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="221fe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="221fe-127">応答</span><span class="sxs-lookup"><span data-stu-id="221fe-127">Response</span></span>

<span data-ttu-id="221fe-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[teamsAppInstallation](../resources/teamsappinstallation.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="221fe-128">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="221fe-129">例</span><span class="sxs-lookup"><span data-stu-id="221fe-129">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="221fe-130">例 1: インストールされているアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="221fe-130">Example 1: List installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="221fe-131">要求</span><span class="sxs-lookup"><span data-stu-id="221fe-131">Request</span></span>

<span data-ttu-id="221fe-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="221fe-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="221fe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="221fe-134">C#</span><span class="sxs-lookup"><span data-stu-id="221fe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="221fe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="221fe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="221fe-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="221fe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="221fe-137">応答</span><span class="sxs-lookup"><span data-stu-id="221fe-137">Response</span></span>

<span data-ttu-id="221fe-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-138">The following is an example of the response.</span></span>
><span data-ttu-id="221fe-139">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="221fe-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="221fe-140">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="221fe-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="221fe-141">例 2: インストールされているアプリの名前とその他の詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="221fe-141">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="221fe-142">要求</span><span class="sxs-lookup"><span data-stu-id="221fe-142">Request</span></span>

<span data-ttu-id="221fe-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-143">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="221fe-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="221fe-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="221fe-145">C#</span><span class="sxs-lookup"><span data-stu-id="221fe-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="221fe-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="221fe-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="221fe-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="221fe-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="221fe-148">応答</span><span class="sxs-lookup"><span data-stu-id="221fe-148">Response</span></span>

<span data-ttu-id="221fe-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-149">The following is an example of the response.</span></span>

><span data-ttu-id="221fe-150">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="221fe-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="221fe-151">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="221fe-151">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
