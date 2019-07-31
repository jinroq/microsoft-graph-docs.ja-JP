---
title: チームのアプリを一覧表示する
description: 指定したチームにインストールされているアプリのリストを取得します。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cd4901aeae8b963c588f8c4671ef75ba09a3ba4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990772"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="ff450-103">チームのアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ff450-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff450-104">指定した[チーム](../resources/team.md)に[インストールされているアプリ](../resources/teamsappinstallation.md)のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff450-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff450-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff450-105">Permissions</span></span>

<span data-ttu-id="ff450-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff450-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff450-108">Permission type</span></span>      | <span data-ttu-id="ff450-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff450-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff450-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff450-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff450-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff450-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff450-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff450-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff450-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff450-113">Not supported.</span></span>    |
|<span data-ttu-id="ff450-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff450-114">Application</span></span> | <span data-ttu-id="ff450-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff450-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ff450-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff450-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff450-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff450-117">Optional query parameters</span></span>

<span data-ttu-id="ff450-118">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリパラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ff450-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff450-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff450-119">Request headers</span></span>

| <span data-ttu-id="ff450-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff450-120">Header</span></span>       | <span data-ttu-id="ff450-121">値</span><span class="sxs-lookup"><span data-stu-id="ff450-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff450-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff450-122">Authorization</span></span>  | <span data-ttu-id="ff450-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff450-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff450-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff450-125">Request body</span></span>

<span data-ttu-id="ff450-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff450-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff450-127">応答</span><span class="sxs-lookup"><span data-stu-id="ff450-127">Response</span></span>

<span data-ttu-id="ff450-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[teamsAppInstallation](../resources/teamsappinstallation.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ff450-128">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff450-129">例</span><span class="sxs-lookup"><span data-stu-id="ff450-129">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="ff450-130">例 1: インストールされているアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ff450-130">Example 1: List installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="ff450-131">要求</span><span class="sxs-lookup"><span data-stu-id="ff450-131">Request</span></span>

<span data-ttu-id="ff450-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff450-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff450-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ff450-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="ff450-134">C#</span><span class="sxs-lookup"><span data-stu-id="ff450-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff450-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff450-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff450-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="ff450-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff450-137">Java</span><span class="sxs-lookup"><span data-stu-id="ff450-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ff450-138">応答</span><span class="sxs-lookup"><span data-stu-id="ff450-138">Response</span></span>

<span data-ttu-id="ff450-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff450-139">The following is an example of the response.</span></span>
><span data-ttu-id="ff450-140">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ff450-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff450-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff450-141">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="ff450-142">例 2: インストールされているアプリの名前とその他の詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="ff450-142">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="ff450-143">要求</span><span class="sxs-lookup"><span data-stu-id="ff450-143">Request</span></span>

<span data-ttu-id="ff450-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff450-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff450-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ff450-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff450-146">C#</span><span class="sxs-lookup"><span data-stu-id="ff450-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff450-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff450-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff450-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="ff450-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff450-149">Java</span><span class="sxs-lookup"><span data-stu-id="ff450-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff450-150">応答</span><span class="sxs-lookup"><span data-stu-id="ff450-150">Response</span></span>

<span data-ttu-id="ff450-151">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff450-151">The following is an example of the response.</span></span>

><span data-ttu-id="ff450-152">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ff450-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff450-153">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff450-153">All the properties will be returned from an actual call.</span></span>
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
