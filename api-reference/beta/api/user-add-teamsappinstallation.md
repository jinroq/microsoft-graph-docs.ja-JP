---
title: ユーザー用のアプリをインストールする
description: 指定したユーザーの個人スコープにアプリをインストールします。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 009d2efe115d8b07f9bdead07965d402db65e65a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908545"
---
# <a name="install-app-for-user"></a><span data-ttu-id="60e9d-103">ユーザー用のアプリをインストールする</span><span class="sxs-lookup"><span data-stu-id="60e9d-103">Install app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e9d-104">指定した[ユーザー](../resources/user.md)の個人スコープに[アプリ](../resources/teamsapp.md)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="60e9d-104">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="60e9d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60e9d-105">Permissions</span></span>

<span data-ttu-id="60e9d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60e9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e9d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60e9d-108">Permission type</span></span>      | <span data-ttu-id="60e9d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60e9d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60e9d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60e9d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="60e9d-111">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e9d-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>     |
|<span data-ttu-id="60e9d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60e9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60e9d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60e9d-113">Not supported.</span></span>    |
|<span data-ttu-id="60e9d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60e9d-114">Application</span></span> | <span data-ttu-id="60e9d-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e9d-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60e9d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60e9d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="60e9d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60e9d-117">Request headers</span></span>

| <span data-ttu-id="60e9d-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60e9d-118">Header</span></span>       | <span data-ttu-id="60e9d-119">値</span><span class="sxs-lookup"><span data-stu-id="60e9d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60e9d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60e9d-120">Authorization</span></span>  | <span data-ttu-id="60e9d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60e9d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60e9d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60e9d-123">Request body</span></span>

<span data-ttu-id="60e9d-124">要求本文には、追加する既存のカタログアプリの ID が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60e9d-124">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="60e9d-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60e9d-125">Property</span></span>   | <span data-ttu-id="60e9d-126">型</span><span class="sxs-lookup"><span data-stu-id="60e9d-126">Type</span></span> |<span data-ttu-id="60e9d-127">説明</span><span class="sxs-lookup"><span data-stu-id="60e9d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60e9d-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="60e9d-128">teamsApp</span></span>|<span data-ttu-id="60e9d-129">String</span><span class="sxs-lookup"><span data-stu-id="60e9d-129">String</span></span>|<span data-ttu-id="60e9d-130">追加するアプリの ID。</span><span class="sxs-lookup"><span data-stu-id="60e9d-130">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="60e9d-131">応答</span><span class="sxs-lookup"><span data-stu-id="60e9d-131">Response</span></span>

<span data-ttu-id="60e9d-p103">成功した場合、このメソッドは `201 Created` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="60e9d-p103">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e9d-134">例</span><span class="sxs-lookup"><span data-stu-id="60e9d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="60e9d-135">要求</span><span class="sxs-lookup"><span data-stu-id="60e9d-135">Request</span></span>

<span data-ttu-id="60e9d-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60e9d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="60e9d-137">応答</span><span class="sxs-lookup"><span data-stu-id="60e9d-137">Response</span></span>

<span data-ttu-id="60e9d-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60e9d-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
