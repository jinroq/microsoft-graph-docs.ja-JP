---
title: ユーザー用にインストールされているアプリを一覧表示する
description: 指定したユーザーの個人スコープにインストールされているアプリの一覧を取得します。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c31e731aba27fff245ecd92fc9d93d20d2c1fe27
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908552"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="7c1c6-103">ユーザー用にインストールされているアプリを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7c1c6-103">List apps installed for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c1c6-104">指定した[ユーザー](../resources/user.md)の個人スコープにインストールされている[アプリ](../resources/teamsappinstallation.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-104">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c1c6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c1c6-105">Permissions</span></span>

<span data-ttu-id="7c1c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c1c6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c1c6-108">Permission type</span></span>      | <span data-ttu-id="7c1c6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c1c6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c1c6-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c1c6-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c1c6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c1c6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-113">Not supported.</span></span>    |
|<span data-ttu-id="7c1c6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c1c6-114">Application</span></span> | <span data-ttu-id="7c1c6-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c1c6-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7c1c6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c1c6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c1c6-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c1c6-117">Optional query parameters</span></span>

<span data-ttu-id="7c1c6-118">このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c1c6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c1c6-119">Request headers</span></span>

| <span data-ttu-id="7c1c6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c1c6-120">Header</span></span>       | <span data-ttu-id="7c1c6-121">値</span><span class="sxs-lookup"><span data-stu-id="7c1c6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c1c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c1c6-122">Authorization</span></span>  | <span data-ttu-id="7c1c6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c1c6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c1c6-125">Request body</span></span>

<span data-ttu-id="7c1c6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c1c6-127">応答</span><span class="sxs-lookup"><span data-stu-id="7c1c6-127">Response</span></span>

<span data-ttu-id="7c1c6-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[teamsAppInstallation](../resources/teamsappinstallation.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-128">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c1c6-129">例</span><span class="sxs-lookup"><span data-stu-id="7c1c6-129">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="7c1c6-130">例 1: 指定したユーザー用にインストールされているアプリの一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="7c1c6-130">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="7c1c6-131">要求</span><span class="sxs-lookup"><span data-stu-id="7c1c6-131">Request</span></span>

<span data-ttu-id="7c1c6-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
```

#### <a name="response"></a><span data-ttu-id="7c1c6-133">応答</span><span class="sxs-lookup"><span data-stu-id="7c1c6-133">Response</span></span>

<span data-ttu-id="7c1c6-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-134">The following is an example of the response.</span></span>
><span data-ttu-id="7c1c6-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
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
### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="7c1c6-137">例 2: ユーザーに対してインストールされているアプリの名前とその他の詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="7c1c6-137">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="7c1c6-138">要求</span><span class="sxs-lookup"><span data-stu-id="7c1c6-138">Request</span></span>

<span data-ttu-id="7c1c6-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="7c1c6-140">応答</span><span class="sxs-lookup"><span data-stu-id="7c1c6-140">Response</span></span>

<span data-ttu-id="7c1c6-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-141">The following is an example of the response.</span></span>

><span data-ttu-id="7c1c6-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7c1c6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
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
<!-- {
  "type": "#page.annotation",
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
