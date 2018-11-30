---
title: グループ設定の一覧表示
description: グループ設定オブジェクトのリストを取得します。
ms.openlocfilehash: 2a34627f057a5244a94d7f9e14dde5df1fe12202
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022107"
---
# <a name="list-group-settings"></a><span data-ttu-id="9d304-103">グループ設定の一覧表示</span><span class="sxs-lookup"><span data-stu-id="9d304-103">List group settings</span></span>

<span data-ttu-id="9d304-104">グループ設定オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9d304-104">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d304-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9d304-105">Permissions</span></span>

<span data-ttu-id="9d304-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d304-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d304-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d304-108">Permission type</span></span>      | <span data-ttu-id="9d304-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d304-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d304-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d304-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d304-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d304-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d304-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d304-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d304-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d304-113">Not supported.</span></span>    |
|<span data-ttu-id="9d304-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d304-114">Application</span></span> | <span data-ttu-id="9d304-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d304-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d304-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d304-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="9d304-117">テナント全体またはグループ設定を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9d304-117">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d304-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d304-118">Optional query parameters</span></span>
<span data-ttu-id="9d304-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9d304-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="9d304-120">注: $filter はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d304-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d304-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d304-121">Request headers</span></span>
| <span data-ttu-id="9d304-122">名前</span><span class="sxs-lookup"><span data-stu-id="9d304-122">Name</span></span> | <span data-ttu-id="9d304-123">説明</span><span class="sxs-lookup"><span data-stu-id="9d304-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="9d304-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d304-124">Authorization</span></span>  | <span data-ttu-id="9d304-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9d304-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d304-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d304-127">Request body</span></span>
<span data-ttu-id="9d304-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d304-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d304-129">応答</span><span class="sxs-lookup"><span data-stu-id="9d304-129">Response</span></span>

<span data-ttu-id="9d304-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9d304-130">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d304-131">例</span><span class="sxs-lookup"><span data-stu-id="9d304-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9d304-132">要求</span><span class="sxs-lookup"><span data-stu-id="9d304-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="9d304-133">応答</span><span class="sxs-lookup"><span data-stu-id="9d304-133">Response</span></span>

<span data-ttu-id="9d304-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d304-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->