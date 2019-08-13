---
title: ディレクトリの設定を一覧表示する
description: ディレクトリ設定オブジェクトの一覧を取得します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f2704340a0f6366329bae9074e0e0d206146333e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319455"
---
# <a name="list-directory-settings"></a><span data-ttu-id="fa384-103">ディレクトリの設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fa384-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa384-104">ディレクトリ設定オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="fa384-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="fa384-105">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fa384-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="fa384-106">この API の/v1.0 バージョンは、[ *groupSettings]* の名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="fa384-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa384-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa384-107">Permissions</span></span>
<span data-ttu-id="fa384-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa384-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa384-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa384-110">Permission type</span></span>      | <span data-ttu-id="fa384-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa384-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa384-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa384-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa384-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa384-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa384-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa384-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa384-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa384-115">Not supported.</span></span>    |
|<span data-ttu-id="fa384-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa384-116">Application</span></span> | <span data-ttu-id="fa384-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa384-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa384-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa384-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fa384-119">テナント全体またはグループ設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="fa384-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa384-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fa384-120">Optional query parameters</span></span>
<span data-ttu-id="fa384-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fa384-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa384-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa384-122">Request headers</span></span>
| <span data-ttu-id="fa384-123">名前</span><span class="sxs-lookup"><span data-stu-id="fa384-123">Name</span></span>      |<span data-ttu-id="fa384-124">説明</span><span class="sxs-lookup"><span data-stu-id="fa384-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa384-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa384-125">Authorization</span></span>  | <span data-ttu-id="fa384-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fa384-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa384-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa384-128">Request body</span></span>
<span data-ttu-id="fa384-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa384-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa384-130">応答</span><span class="sxs-lookup"><span data-stu-id="fa384-130">Response</span></span>

<span data-ttu-id="fa384-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directorysetting](../resources/directorysetting.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fa384-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa384-132">例</span><span class="sxs-lookup"><span data-stu-id="fa384-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa384-133">要求</span><span class="sxs-lookup"><span data-stu-id="fa384-133">Request</span></span>
<span data-ttu-id="fa384-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa384-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa384-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fa384-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa384-136">C#</span><span class="sxs-lookup"><span data-stu-id="fa384-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa384-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa384-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa384-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="fa384-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa384-139">Java</span><span class="sxs-lookup"><span data-stu-id="fa384-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa384-140">応答</span><span class="sxs-lookup"><span data-stu-id="fa384-140">Response</span></span>
<span data-ttu-id="fa384-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa384-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "settingTemplateId": "settingTemplateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
