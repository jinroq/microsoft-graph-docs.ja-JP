---
title: メンバーを一覧表示する
description: ディレクトリ ロールに割り当てられているユーザーの一覧を取得します。ディレクトリに割り当てることができるのはユーザーのみです。
author: lleonard-msft
ms.openlocfilehash: 4fdbb5fd940e9fa20adb9f2a3d3dd1c7c035dbf7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359886"
---
# <a name="list-members"></a><span data-ttu-id="4a385-104">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4a385-104">List members</span></span>

<span data-ttu-id="4a385-p102">ディレクトリ ロールに割り当てられているユーザーの一覧を取得します。ディレクトリに割り当てることができるのはユーザーのみです。</span><span class="sxs-lookup"><span data-stu-id="4a385-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a385-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a385-107">Permissions</span></span>
<span data-ttu-id="4a385-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a385-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a385-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a385-110">Permission type</span></span>      | <span data-ttu-id="4a385-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a385-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a385-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a385-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a385-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a385-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a385-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a385-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a385-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a385-115">Not supported.</span></span>    |
|<span data-ttu-id="4a385-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a385-116">Application</span></span> | <span data-ttu-id="4a385-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a385-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a385-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a385-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a385-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a385-119">Optional query parameters</span></span>
<span data-ttu-id="4a385-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4a385-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4a385-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a385-121">Request headers</span></span>
| <span data-ttu-id="4a385-122">名前</span><span class="sxs-lookup"><span data-stu-id="4a385-122">Name</span></span>       | <span data-ttu-id="4a385-123">種類</span><span class="sxs-lookup"><span data-stu-id="4a385-123">Type</span></span> | <span data-ttu-id="4a385-124">説明</span><span class="sxs-lookup"><span data-stu-id="4a385-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4a385-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a385-125">Authorization</span></span>  | <span data-ttu-id="4a385-126">string</span><span class="sxs-lookup"><span data-stu-id="4a385-126">string</span></span>  | <span data-ttu-id="4a385-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a385-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a385-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a385-129">Request body</span></span>
<span data-ttu-id="4a385-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4a385-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a385-131">応答</span><span class="sxs-lookup"><span data-stu-id="4a385-131">Response</span></span>

<span data-ttu-id="4a385-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4a385-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a385-133">例</span><span class="sxs-lookup"><span data-stu-id="4a385-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a385-134">要求</span><span class="sxs-lookup"><span data-stu-id="4a385-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="4a385-135">応答</span><span class="sxs-lookup"><span data-stu-id="4a385-135">Response</span></span>
<span data-ttu-id="4a385-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a385-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->