---
title: groupSettingTemplates のリスト
description: グループ設定テンプレートは、テナント内でグループ設定を作成および使用するための一連のテンプレートを表します。この操作は、使用可能な groupSettingTemplates オブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bd34c3004211243c0146f5c0200bcdf2fb821600
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447384"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="54cf8-104">groupSettingTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="54cf8-104">List groupSettingTemplates</span></span>

<span data-ttu-id="54cf8-p102">グループ設定テンプレートは、テナント内でグループ設定を作成および使用するための一連のテンプレートを表します。この操作は、使用可能な groupSettingTemplates オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="54cf8-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="54cf8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54cf8-107">Permissions</span></span>

<span data-ttu-id="54cf8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54cf8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54cf8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54cf8-110">Permission type</span></span>      | <span data-ttu-id="54cf8-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="54cf8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54cf8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54cf8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54cf8-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54cf8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54cf8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54cf8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54cf8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54cf8-115">Not supported.</span></span>    |
|<span data-ttu-id="54cf8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54cf8-116">Application</span></span> | <span data-ttu-id="54cf8-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54cf8-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54cf8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54cf8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54cf8-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="54cf8-119">Optional query parameters</span></span>
<span data-ttu-id="54cf8-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="54cf8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="54cf8-121">**注:** $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54cf8-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54cf8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54cf8-122">Request headers</span></span>
| <span data-ttu-id="54cf8-123">名前</span><span class="sxs-lookup"><span data-stu-id="54cf8-123">Name</span></span> | <span data-ttu-id="54cf8-124">説明</span><span class="sxs-lookup"><span data-stu-id="54cf8-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="54cf8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="54cf8-125">Authorization</span></span>  | <span data-ttu-id="54cf8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="54cf8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54cf8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="54cf8-128">Request body</span></span>
<span data-ttu-id="54cf8-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54cf8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54cf8-130">応答</span><span class="sxs-lookup"><span data-stu-id="54cf8-130">Response</span></span>

<span data-ttu-id="54cf8-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSettingTemplate](../resources/groupsettingtemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="54cf8-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54cf8-132">例</span><span class="sxs-lookup"><span data-stu-id="54cf8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54cf8-133">要求</span><span class="sxs-lookup"><span data-stu-id="54cf8-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="54cf8-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="54cf8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54cf8-135">C#</span><span class="sxs-lookup"><span data-stu-id="54cf8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54cf8-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="54cf8-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54cf8-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="54cf8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54cf8-138">応答</span><span class="sxs-lookup"><span data-stu-id="54cf8-138">Response</span></span>

<span data-ttu-id="54cf8-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54cf8-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
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
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
