---
title: グループ設定テンプレートを取得する
description: グループ設定テンプレートは、テナント内で設定を作成することができる設定のテンプレートを表します。 この操作により、使用可能な設定とその既定値を含む groupSettingTemplate オブジェクトのプロパティを取得できるようになります。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1f90914f7a381e8be2d4bc0dd4e3a5460ce1015
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277127"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="b5d2b-104">グループ設定テンプレートを取得する</span><span class="sxs-lookup"><span data-stu-id="b5d2b-104">Get a group setting template</span></span>

<span data-ttu-id="b5d2b-p102">グループ設定テンプレートは、テナント内で作成できる設定に基づいた設定のテンプレートを表します。この操作により、利用可能な設定とその既定値を含む、[groupSettingTemplate](../resources/groupsettingtemplate.md) オブジェクトのプロパティを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-p102">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5d2b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b5d2b-107">Permissions</span></span>

<span data-ttu-id="b5d2b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5d2b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5d2b-110">Permission type</span></span>      | <span data-ttu-id="b5d2b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5d2b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5d2b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5d2b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b5d2b-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5d2b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5d2b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5d2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d2b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-115">Not supported.</span></span>    |
|<span data-ttu-id="b5d2b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5d2b-116">Application</span></span> | <span data-ttu-id="b5d2b-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d2b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5d2b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5d2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5d2b-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b5d2b-119">Optional query parameters</span></span>
<span data-ttu-id="b5d2b-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5d2b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5d2b-121">Request headers</span></span>
| <span data-ttu-id="b5d2b-122">名前</span><span class="sxs-lookup"><span data-stu-id="b5d2b-122">Name</span></span> | <span data-ttu-id="b5d2b-123">説明</span><span class="sxs-lookup"><span data-stu-id="b5d2b-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b5d2b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d2b-124">Authorization</span></span> | <span data-ttu-id="b5d2b-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5d2b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5d2b-127">Request body</span></span>
<span data-ttu-id="b5d2b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5d2b-129">応答</span><span class="sxs-lookup"><span data-stu-id="b5d2b-129">Response</span></span>

<span data-ttu-id="b5d2b-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSettingTemplate](../resources/groupsettingtemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5d2b-131">例</span><span class="sxs-lookup"><span data-stu-id="b5d2b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5d2b-132">要求</span><span class="sxs-lookup"><span data-stu-id="b5d2b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="b5d2b-133">応答</span><span class="sxs-lookup"><span data-stu-id="b5d2b-133">Response</span></span>

<span data-ttu-id="b5d2b-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b5d2b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "deletedDateTime": null,
    "displayName": "Group.Unified",
    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
    "values": [
        {
            "name": "CustomBlockedWordsList",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "type": "System.Boolean",
            "defaultValue": "false",
            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "ClassificationDescriptions",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5d2b-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="b5d2b-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5d2b-137">C#</span><span class="sxs-lookup"><span data-stu-id="b5d2b-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5d2b-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5d2b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b5d2b-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="b5d2b-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
