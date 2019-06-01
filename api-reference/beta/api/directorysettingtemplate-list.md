---
title: DirectorySettingTemplates を一覧表示する
description: ディレクトリ設定テンプレートは、ディレクトリ設定のテンプレートのセットを表します。これは、テナント内でディレクトリ設定を作成して使用することができます。  この操作により、使用可能な directorySettingTemplates オブジェクトの一覧が取得されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adfb303e24b637af4b77ac9f3cfd357ca09ece8f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655783"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="4484d-104">DirectorySettingTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4484d-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4484d-105">ディレクトリ設定テンプレートは、ディレクトリ設定のテンプレートのセットを表します。これは、テナント内でディレクトリ設定を作成して使用することができます。</span><span class="sxs-lookup"><span data-stu-id="4484d-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="4484d-106">この操作により、使用可能な directorySettingTemplates オブジェクトの一覧が取得されます。</span><span class="sxs-lookup"><span data-stu-id="4484d-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="4484d-107">**注**: この API のベータ版は、グループにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4484d-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="4484d-108">この API の/v1.0 バージョンは、" *groupSettingTemplate List*" という名前に変更されました。</span><span class="sxs-lookup"><span data-stu-id="4484d-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="4484d-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4484d-109">Permissions</span></span>
<span data-ttu-id="4484d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4484d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4484d-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4484d-112">Permission type</span></span>      | <span data-ttu-id="4484d-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4484d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4484d-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4484d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4484d-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4484d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4484d-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4484d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4484d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4484d-117">Not supported.</span></span>    |
|<span data-ttu-id="4484d-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4484d-118">Application</span></span> | <span data-ttu-id="4484d-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4484d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4484d-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4484d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4484d-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4484d-121">Optional query parameters</span></span>
<span data-ttu-id="4484d-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4484d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4484d-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4484d-123">Request headers</span></span>
| <span data-ttu-id="4484d-124">名前</span><span class="sxs-lookup"><span data-stu-id="4484d-124">Name</span></span>      |<span data-ttu-id="4484d-125">説明</span><span class="sxs-lookup"><span data-stu-id="4484d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4484d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4484d-126">Authorization</span></span>  | <span data-ttu-id="4484d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4484d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4484d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4484d-129">Request body</span></span>
<span data-ttu-id="4484d-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4484d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4484d-131">応答</span><span class="sxs-lookup"><span data-stu-id="4484d-131">Response</span></span>

<span data-ttu-id="4484d-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directorysettingtemplate](../resources/directorysettingtemplate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4484d-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4484d-133">例</span><span class="sxs-lookup"><span data-stu-id="4484d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4484d-134">要求</span><span class="sxs-lookup"><span data-stu-id="4484d-134">Request</span></span>
<span data-ttu-id="4484d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4484d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="4484d-136">応答</span><span class="sxs-lookup"><span data-stu-id="4484d-136">Response</span></span>
<span data-ttu-id="4484d-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4484d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4484d-140">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="4484d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4484d-141">C#</span><span class="sxs-lookup"><span data-stu-id="4484d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4484d-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="4484d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
