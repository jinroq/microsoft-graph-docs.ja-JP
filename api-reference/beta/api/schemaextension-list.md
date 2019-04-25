---
title: schemaExtensions を一覧表示する
description: '現在のテナントで所有しているすべてのアプリによって作成された schemaextension オブジェクトの一覧を取得します ( '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a320cc0261c40ee8b87dcc658c6ca146d77190e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537777"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="19527-103">schemaExtensions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="19527-103">List schemaExtensions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19527-104">現在のテナントで所有しているすべてのアプリによって作成された[schemaextension](../resources/schemaextension.md)オブジェクトの一覧を取得します (これは、**開発**中、**使用可能**、または**廃止**され**た場合があります)。また、その他のアプリが所有するすべてのスキーマ拡張機能利用可能**です。</span><span class="sxs-lookup"><span data-stu-id="19527-104">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="19527-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19527-105">Permissions</span></span>
<span data-ttu-id="19527-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19527-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19527-108">Permission type</span></span>      | <span data-ttu-id="19527-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19527-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19527-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19527-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19527-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19527-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19527-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19527-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19527-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19527-113">Not supported.</span></span>    |
|<span data-ttu-id="19527-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19527-114">Application</span></span> | <span data-ttu-id="19527-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="19527-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19527-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19527-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19527-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="19527-117">Optional query parameters</span></span>
<span data-ttu-id="19527-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="19527-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19527-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19527-119">Request headers</span></span>
| <span data-ttu-id="19527-120">名前</span><span class="sxs-lookup"><span data-stu-id="19527-120">Name</span></span>      |<span data-ttu-id="19527-121">説明</span><span class="sxs-lookup"><span data-stu-id="19527-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19527-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19527-122">Authorization</span></span>  | <span data-ttu-id="19527-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19527-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19527-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19527-125">Content-Type</span></span>   | <span data-ttu-id="19527-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19527-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19527-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="19527-127">Request body</span></span>
<span data-ttu-id="19527-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="19527-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19527-129">応答</span><span class="sxs-lookup"><span data-stu-id="19527-129">Response</span></span>

<span data-ttu-id="19527-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schemaextension](../resources/schemaextension.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="19527-130">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19527-131">例</span><span class="sxs-lookup"><span data-stu-id="19527-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19527-132">要求</span><span class="sxs-lookup"><span data-stu-id="19527-132">Request</span></span>
<span data-ttu-id="19527-133">次の例は、一意の**id**でフィルター処理することによって、特定のアクセス可能なすべての拡張機能を確認する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="19527-133">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="19527-134">応答</span><span class="sxs-lookup"><span data-stu-id="19527-134">Response</span></span>
<span data-ttu-id="19527-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="19527-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
    {
      "id":"graphlearn_test",
      "description": "Yet another test schema",
      "targetTypes": [
          "User", "Group"
      ],
      "status": "InDevelopment",
      "owner": "24d3b144-21ae-4080-943f-7067b395b913",
      "properties": [
          {
              "name": "testName",
              "type": "String"
          }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="19527-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="19527-138">See also</span></span>

- [<span data-ttu-id="19527-139">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="19527-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="19527-140">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="19527-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
