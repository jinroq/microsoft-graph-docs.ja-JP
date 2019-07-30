---
title: アプリをチームに追加する
description: 指定したチームにアプリをインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 86902435cad896256775711f48dd4a531adce8f9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931701"
---
# <a name="add-app-to-team"></a><span data-ttu-id="d5794-103">アプリをチームに追加する</span><span class="sxs-lookup"><span data-stu-id="d5794-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5794-104">指定した[チーム](../resources/team.md)に[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="d5794-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5794-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5794-105">Permissions</span></span>

<span data-ttu-id="d5794-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5794-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5794-108">Permission type</span></span>      | <span data-ttu-id="d5794-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5794-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5794-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5794-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5794-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5794-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5794-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5794-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5794-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5794-113">Not supported.</span></span>    |
|<span data-ttu-id="d5794-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5794-114">Application</span></span> | <span data-ttu-id="d5794-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5794-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5794-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5794-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d5794-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5794-117">Request headers</span></span>

| <span data-ttu-id="d5794-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5794-118">Header</span></span>       | <span data-ttu-id="d5794-119">値</span><span class="sxs-lookup"><span data-stu-id="d5794-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d5794-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5794-120">Authorization</span></span>  | <span data-ttu-id="d5794-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5794-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5794-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5794-123">Request body</span></span>

| <span data-ttu-id="d5794-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5794-124">Property</span></span>   | <span data-ttu-id="d5794-125">型</span><span class="sxs-lookup"><span data-stu-id="d5794-125">Type</span></span> |<span data-ttu-id="d5794-126">説明</span><span class="sxs-lookup"><span data-stu-id="d5794-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5794-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d5794-127">teamsApp</span></span>|<span data-ttu-id="d5794-128">String</span><span class="sxs-lookup"><span data-stu-id="d5794-128">String</span></span>|<span data-ttu-id="d5794-129">追加するアプリの id。</span><span class="sxs-lookup"><span data-stu-id="d5794-129">The id of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="d5794-130">応答</span><span class="sxs-lookup"><span data-stu-id="d5794-130">Response</span></span>

<span data-ttu-id="d5794-p103">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d5794-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5794-133">例</span><span class="sxs-lookup"><span data-stu-id="d5794-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5794-134">要求</span><span class="sxs-lookup"><span data-stu-id="d5794-134">Request</span></span>

<span data-ttu-id="d5794-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5794-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d5794-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d5794-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_teamsApp"
}-->
```http
POST /teams/87654321-0abc-zqf0-321456789q/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5794-137">C#</span><span class="sxs-lookup"><span data-stu-id="d5794-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5794-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5794-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5794-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="d5794-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5794-140">Java</span><span class="sxs-lookup"><span data-stu-id="d5794-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5794-141">応答</span><span class="sxs-lookup"><span data-stu-id="d5794-141">Response</span></span>

<span data-ttu-id="d5794-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d5794-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add teamsApp",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
