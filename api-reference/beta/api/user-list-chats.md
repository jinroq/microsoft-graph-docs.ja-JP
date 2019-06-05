---
title: チャットの一覧表示
description: チャットオブジェクトの一覧を取得します。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b00e316c568ef6432cb4127b9f3ce1295cd8971
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720936"
---
# <a name="list-chats"></a><span data-ttu-id="b6fad-103">チャットの一覧表示</span><span class="sxs-lookup"><span data-stu-id="b6fad-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6fad-104">チャットオブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b6fad-104">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6fad-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6fad-105">Permissions</span></span>

<span data-ttu-id="b6fad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6fad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6fad-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6fad-108">Permission type</span></span>                        | <span data-ttu-id="b6fad-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6fad-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b6fad-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6fad-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6fad-111">チャット。読み取り、読み取り/書き込み</span><span class="sxs-lookup"><span data-stu-id="b6fad-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="b6fad-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6fad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6fad-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6fad-113">Not supported.</span></span> |
| <span data-ttu-id="b6fad-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6fad-114">Application</span></span>                            | <span data-ttu-id="b6fad-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6fad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6fad-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6fad-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6fad-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b6fad-117">Optional query parameters</span></span>

<span data-ttu-id="b6fad-118">この操作では、応答をカスタマイズするための[OData クエリパラメーター](/graph/query-parameters)をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="b6fad-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6fad-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6fad-119">Request headers</span></span>

| <span data-ttu-id="b6fad-120">名前</span><span class="sxs-lookup"><span data-stu-id="b6fad-120">Name</span></span>      |<span data-ttu-id="b6fad-121">説明</span><span class="sxs-lookup"><span data-stu-id="b6fad-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6fad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6fad-122">Authorization</span></span> | <span data-ttu-id="b6fad-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b6fad-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6fad-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6fad-124">Request body</span></span>

<span data-ttu-id="b6fad-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6fad-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6fad-126">応答</span><span class="sxs-lookup"><span data-stu-id="b6fad-126">Response</span></span>

<span data-ttu-id="b6fad-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [chat](../resources/chat.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b6fad-127">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6fad-128">例</span><span class="sxs-lookup"><span data-stu-id="b6fad-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6fad-129">要求</span><span class="sxs-lookup"><span data-stu-id="b6fad-129">Request</span></span>

<span data-ttu-id="b6fad-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6fad-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

### <a name="response"></a><span data-ttu-id="b6fad-131">応答</span><span class="sxs-lookup"><span data-stu-id="b6fad-131">Response</span></span>

<span data-ttu-id="b6fad-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b6fad-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b6fad-133">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="b6fad-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6fad-134">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b6fad-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "topic": "topic-value",
      "createdDateTime": "datetime-value",
      "lastUpdatedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->