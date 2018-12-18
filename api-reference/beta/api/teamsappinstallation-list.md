---
title: チームでのアプリケーションの一覧
description: 指定されたチームにインストールされているアプリケーションの一覧を取得します。
author: nkramer
ms.openlocfilehash: d412085663a67a16fe435c8555d802cec662a23e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357289"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="18b14-103">チームでのアプリケーションの一覧</span><span class="sxs-lookup"><span data-stu-id="18b14-103">List apps in team</span></span>

> <span data-ttu-id="18b14-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18b14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18b14-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b14-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18b14-106">[アプリケーションのインストール](../resources/teamsappinstallation.md)を指定された[チーム](../resources/team.md)での一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="18b14-106">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18b14-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18b14-107">Permissions</span></span>

<span data-ttu-id="18b14-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18b14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18b14-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18b14-110">Permission type</span></span>      | <span data-ttu-id="18b14-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18b14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18b14-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18b14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18b14-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b14-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18b14-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18b14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18b14-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b14-115">Not supported.</span></span>    |
|<span data-ttu-id="18b14-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18b14-116">Application</span></span> | <span data-ttu-id="18b14-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b14-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18b14-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18b14-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18b14-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="18b14-119">Optional query parameters</span></span>

<span data-ttu-id="18b14-120">このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。</span><span class="sxs-lookup"><span data-stu-id="18b14-120">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18b14-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b14-121">Request headers</span></span>

| <span data-ttu-id="18b14-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b14-122">Header</span></span>       | <span data-ttu-id="18b14-123">値</span><span class="sxs-lookup"><span data-stu-id="18b14-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18b14-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b14-124">Authorization</span></span>  | <span data-ttu-id="18b14-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18b14-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18b14-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18b14-127">Request body</span></span>

<span data-ttu-id="18b14-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18b14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18b14-129">応答</span><span class="sxs-lookup"><span data-stu-id="18b14-129">Response</span></span>

<span data-ttu-id="18b14-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[teamsApp](../resources/teamsapp.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="18b14-130">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b14-131">例</span><span class="sxs-lookup"><span data-stu-id="18b14-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18b14-132">要求</span><span class="sxs-lookup"><span data-stu-id="18b14-132">Request</span></span>

<span data-ttu-id="18b14-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18b14-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="18b14-134">応答</span><span class="sxs-lookup"><span data-stu-id="18b14-134">Response</span></span>

<span data-ttu-id="18b14-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18b14-135">The following is an example of the response.</span></span>
><span data-ttu-id="18b14-136">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="18b14-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18b14-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="18b14-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="18b14-138">例--は、インストールされているアプリケーションの名前を取得します。</span><span class="sxs-lookup"><span data-stu-id="18b14-138">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="18b14-139">要求</span><span class="sxs-lookup"><span data-stu-id="18b14-139">Request</span></span>

<span data-ttu-id="18b14-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18b14-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="18b14-141">応答</span><span class="sxs-lookup"><span data-stu-id="18b14-141">Response</span></span>

<span data-ttu-id="18b14-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18b14-142">The following is an example of the response.</span></span>

><span data-ttu-id="18b14-143">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="18b14-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18b14-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="18b14-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->