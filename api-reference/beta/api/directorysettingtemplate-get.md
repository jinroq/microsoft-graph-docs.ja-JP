---
title: ディレクトリ設定テンプレートを取得する
description: ディレクトリ設定テンプレートは、テナント内で設定を作成することができる設定のテンプレートを表します。 この操作により、使用可能な設定とその既定値を含む directorySettingTemplate オブジェクトのプロパティを取得できるようになります。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75ead2b0f61e7a9b51ad86571a13703e6ef34780
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957529"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="284c4-104">ディレクトリ設定テンプレートを取得する</span><span class="sxs-lookup"><span data-stu-id="284c4-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="284c4-105">ディレクトリ設定テンプレートは、テナント内で設定を作成することができる設定のテンプレートを表します。</span><span class="sxs-lookup"><span data-stu-id="284c4-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="284c4-106">この操作により、使用可能な設定とその既定値を含む directorySettingTemplate オブジェクトのプロパティを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="284c4-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="284c4-107">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="284c4-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="284c4-108">この API の/v1.0 バージョンは、 *groupSettingTemplate を取得*する名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="284c4-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="284c4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="284c4-109">Permissions</span></span>
<span data-ttu-id="284c4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="284c4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="284c4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="284c4-112">Permission type</span></span>      | <span data-ttu-id="284c4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="284c4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="284c4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="284c4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="284c4-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="284c4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="284c4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="284c4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="284c4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="284c4-117">Not supported.</span></span>    |
|<span data-ttu-id="284c4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="284c4-118">Application</span></span> | <span data-ttu-id="284c4-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284c4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="284c4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="284c4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="284c4-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="284c4-121">Optional query parameters</span></span>
<span data-ttu-id="284c4-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="284c4-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="284c4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="284c4-123">Request headers</span></span>
| <span data-ttu-id="284c4-124">名前</span><span class="sxs-lookup"><span data-stu-id="284c4-124">Name</span></span>      |<span data-ttu-id="284c4-125">説明</span><span class="sxs-lookup"><span data-stu-id="284c4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="284c4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="284c4-126">Authorization</span></span>  | <span data-ttu-id="284c4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="284c4-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="284c4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="284c4-129">Request body</span></span>
<span data-ttu-id="284c4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="284c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="284c4-131">応答</span><span class="sxs-lookup"><span data-stu-id="284c4-131">Response</span></span>

<span data-ttu-id="284c4-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directorysettingtemplate](../resources/directorysettingtemplate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="284c4-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="284c4-133">例</span><span class="sxs-lookup"><span data-stu-id="284c4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="284c4-134">要求</span><span class="sxs-lookup"><span data-stu-id="284c4-134">Request</span></span>
<span data-ttu-id="284c4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="284c4-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="284c4-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="284c4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="284c4-137">C#</span><span class="sxs-lookup"><span data-stu-id="284c4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="284c4-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="284c4-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="284c4-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="284c4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="284c4-140">Java</span><span class="sxs-lookup"><span data-stu-id="284c4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="284c4-141">応答</span><span class="sxs-lookup"><span data-stu-id="284c4-141">Response</span></span>
<span data-ttu-id="284c4-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="284c4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

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
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
