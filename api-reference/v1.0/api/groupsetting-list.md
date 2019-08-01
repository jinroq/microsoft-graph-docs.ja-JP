---
title: グループ設定を一覧表示する
description: グループ設定オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4699f58442f66dbff3bfa3e3913266776c7f4ac5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014528"
---
# <a name="list-group-settings"></a><span data-ttu-id="83e07-103">グループ設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="83e07-103">List group settings</span></span>

<span data-ttu-id="83e07-104">グループ設定オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="83e07-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="83e07-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="83e07-105">Permissions</span></span>

<span data-ttu-id="83e07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83e07-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83e07-108">Permission type</span></span>      | <span data-ttu-id="83e07-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="83e07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83e07-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83e07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83e07-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83e07-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83e07-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83e07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e07-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e07-113">Not supported.</span></span>    |
|<span data-ttu-id="83e07-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83e07-114">Application</span></span> | <span data-ttu-id="83e07-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e07-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83e07-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83e07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="83e07-117">テナント全体またはグループ設定を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="83e07-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET groups/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83e07-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="83e07-118">Optional query parameters</span></span>
<span data-ttu-id="83e07-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="83e07-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

><span data-ttu-id="83e07-120">**注:** $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e07-120">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83e07-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83e07-121">Request headers</span></span>
| <span data-ttu-id="83e07-122">名前</span><span class="sxs-lookup"><span data-stu-id="83e07-122">Name</span></span> | <span data-ttu-id="83e07-123">説明</span><span class="sxs-lookup"><span data-stu-id="83e07-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="83e07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e07-124">Authorization</span></span>  | <span data-ttu-id="83e07-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="83e07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83e07-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="83e07-127">Request body</span></span>
<span data-ttu-id="83e07-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83e07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e07-129">応答</span><span class="sxs-lookup"><span data-stu-id="83e07-129">Response</span></span>

<span data-ttu-id="83e07-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[groupsetting](../resources/groupsetting.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="83e07-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83e07-131">例</span><span class="sxs-lookup"><span data-stu-id="83e07-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83e07-132">要求</span><span class="sxs-lookup"><span data-stu-id="83e07-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83e07-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="83e07-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83e07-134">C#</span><span class="sxs-lookup"><span data-stu-id="83e07-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83e07-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="83e07-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83e07-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="83e07-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83e07-137">Java</span><span class="sxs-lookup"><span data-stu-id="83e07-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="83e07-138">応答</span><span class="sxs-lookup"><span data-stu-id="83e07-138">Response</span></span>

<span data-ttu-id="83e07-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83e07-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
