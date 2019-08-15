---
title: DirectorySettingTemplates を一覧表示する
description: ディレクトリ設定テンプレートは、ディレクトリ設定のテンプレートのセットを表します。これは、テナント内でディレクトリ設定を作成して使用することができます。  この操作により、使用可能な directorySettingTemplates オブジェクトの一覧が取得されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4cdb3795e0cab3f3ee66fd47f9f8876e56d9d705
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417138"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="20140-104">DirectorySettingTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="20140-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20140-105">ディレクトリ設定テンプレートは、ディレクトリ設定のテンプレートのセットを表します。これは、テナント内でディレクトリ設定を作成して使用することができます。</span><span class="sxs-lookup"><span data-stu-id="20140-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="20140-106">この操作により、使用可能な directorySettingTemplates オブジェクトの一覧が取得されます。</span><span class="sxs-lookup"><span data-stu-id="20140-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="20140-107">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="20140-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="20140-108">この API の/v1.0 バージョンは、" *groupSettingTemplate List*" という名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="20140-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="20140-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20140-109">Permissions</span></span>
<span data-ttu-id="20140-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20140-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20140-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20140-112">Permission type</span></span>      | <span data-ttu-id="20140-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="20140-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20140-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20140-114">Delegated (work or school account)</span></span> | <span data-ttu-id="20140-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20140-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20140-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20140-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20140-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20140-117">Not supported.</span></span>    |
|<span data-ttu-id="20140-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20140-118">Application</span></span> | <span data-ttu-id="20140-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20140-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20140-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20140-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20140-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="20140-121">Optional query parameters</span></span>
<span data-ttu-id="20140-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="20140-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20140-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20140-123">Request headers</span></span>
| <span data-ttu-id="20140-124">名前</span><span class="sxs-lookup"><span data-stu-id="20140-124">Name</span></span>      |<span data-ttu-id="20140-125">説明</span><span class="sxs-lookup"><span data-stu-id="20140-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20140-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="20140-126">Authorization</span></span>  | <span data-ttu-id="20140-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="20140-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20140-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="20140-129">Request body</span></span>
<span data-ttu-id="20140-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="20140-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20140-131">応答</span><span class="sxs-lookup"><span data-stu-id="20140-131">Response</span></span>

<span data-ttu-id="20140-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directorysettingtemplate](../resources/directorysettingtemplate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="20140-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20140-133">例</span><span class="sxs-lookup"><span data-stu-id="20140-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20140-134">要求</span><span class="sxs-lookup"><span data-stu-id="20140-134">Request</span></span>
<span data-ttu-id="20140-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20140-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20140-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="20140-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20140-137">C#</span><span class="sxs-lookup"><span data-stu-id="20140-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20140-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20140-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20140-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="20140-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20140-140">応答</span><span class="sxs-lookup"><span data-stu-id="20140-140">Response</span></span>
<span data-ttu-id="20140-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20140-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "description": "description-value",
      "values": [
        {
          "name": "name-value",
          "type": "type-value",
          "defaultValue": "defaultValue-value",
          "description": "description-value"
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
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
