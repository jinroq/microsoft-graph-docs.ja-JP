---
title: 'orgContact: 所属するグループ] ボックスの一覧'
description: グループおよび管理の単位のメンバーである連絡先の一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: 318936a49c4eeb56f05c685fc1a1ddd1eaad1a62
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862687"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="c199f-103">orgContact: 所属するグループ] ボックスの一覧</span><span class="sxs-lookup"><span data-stu-id="c199f-103">orgContact: List memberOf</span></span>

> <span data-ttu-id="c199f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c199f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c199f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c199f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c199f-106">グループおよび管理の単位のメンバーである連絡先の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c199f-106">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="c199f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c199f-107">Permissions</span></span>
<span data-ttu-id="c199f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c199f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c199f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c199f-110">Permission type</span></span>      | <span data-ttu-id="c199f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c199f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c199f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c199f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c199f-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c199f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c199f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c199f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c199f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c199f-115">Not supported.</span></span>    |
|<span data-ttu-id="c199f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c199f-116">Application</span></span> | <span data-ttu-id="c199f-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c199f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c199f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c199f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c199f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c199f-119">Optional query parameters</span></span>
<span data-ttu-id="c199f-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c199f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c199f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c199f-121">Request headers</span></span>
| <span data-ttu-id="c199f-122">名前</span><span class="sxs-lookup"><span data-stu-id="c199f-122">Name</span></span>       | <span data-ttu-id="c199f-123">種類</span><span class="sxs-lookup"><span data-stu-id="c199f-123">Type</span></span> | <span data-ttu-id="c199f-124">説明</span><span class="sxs-lookup"><span data-stu-id="c199f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c199f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c199f-125">Authorization</span></span>  | <span data-ttu-id="c199f-126">string</span><span class="sxs-lookup"><span data-stu-id="c199f-126">string</span></span>  | <span data-ttu-id="c199f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c199f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c199f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c199f-129">Request body</span></span>
<span data-ttu-id="c199f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c199f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c199f-131">応答</span><span class="sxs-lookup"><span data-stu-id="c199f-131">Response</span></span>

<span data-ttu-id="c199f-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c199f-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c199f-133">例</span><span class="sxs-lookup"><span data-stu-id="c199f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c199f-134">要求</span><span class="sxs-lookup"><span data-stu-id="c199f-134">Request</span></span>
<span data-ttu-id="c199f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c199f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="c199f-136">応答</span><span class="sxs-lookup"><span data-stu-id="c199f-136">Response</span></span>
<span data-ttu-id="c199f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c199f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
