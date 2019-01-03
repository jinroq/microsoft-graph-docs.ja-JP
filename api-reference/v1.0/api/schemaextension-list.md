---
title: schemaExtensions を一覧表示する
description: '(ことができる現在のテナントで自分が所有する任意のアプリケーションによって作成された schemaExtension オブジェクトのリストを取得します。 '
ms.openlocfilehash: b5e11856156094cc797b9e620c8e2d3ff82da349
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023999"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="7d648-103">schemaExtensions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7d648-103">List schemaExtensions</span></span>

<span data-ttu-id="7d648-104">現在のテナントで所有するアプリによって作成された [schemaExtension](../resources/schemaextension.md) オブジェクト (**InDevelopment**、**Available**、**Deprecated** のもの) と、他のアプリによって所有されていて、**Available** とマークされている他のすべてのスキーマ拡張機能の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7d648-104">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7d648-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d648-105">Permissions</span></span>
<span data-ttu-id="7d648-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d648-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d648-108">Permission type</span></span>      | <span data-ttu-id="7d648-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d648-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d648-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d648-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d648-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d648-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d648-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d648-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d648-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d648-113">Not supported.</span></span>    |
|<span data-ttu-id="7d648-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d648-114">Application</span></span> | <span data-ttu-id="7d648-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d648-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d648-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d648-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d648-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7d648-117">Optional query parameters</span></span>
<span data-ttu-id="7d648-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7d648-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d648-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d648-119">Request headers</span></span>
| <span data-ttu-id="7d648-120">名前</span><span class="sxs-lookup"><span data-stu-id="7d648-120">Name</span></span>      |<span data-ttu-id="7d648-121">説明</span><span class="sxs-lookup"><span data-stu-id="7d648-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d648-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d648-122">Authorization</span></span>  | <span data-ttu-id="7d648-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d648-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d648-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d648-125">Content-Type</span></span>   | <span data-ttu-id="7d648-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d648-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d648-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d648-127">Request body</span></span>
<span data-ttu-id="7d648-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7d648-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d648-129">応答</span><span class="sxs-lookup"><span data-stu-id="7d648-129">Response</span></span>

<span data-ttu-id="7d648-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [schemaExtension](../resources/schemaextension.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7d648-130">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d648-131">例</span><span class="sxs-lookup"><span data-stu-id="7d648-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d648-132">要求</span><span class="sxs-lookup"><span data-stu-id="7d648-132">Request</span></span>
<span data-ttu-id="7d648-133">以下は、一意の **ID** を使用してフィルタリングを行い、すべてのアクセス可能な拡張機能の中から特定の拡張機能を検索する方法の例です。</span><span class="sxs-lookup"><span data-stu-id="7d648-133">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="7d648-134">応答</span><span class="sxs-lookup"><span data-stu-id="7d648-134">Response</span></span>
<span data-ttu-id="7d648-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d648-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7d648-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d648-138">See also</span></span>

- [<span data-ttu-id="7d648-139">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="7d648-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7d648-140">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="7d648-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->