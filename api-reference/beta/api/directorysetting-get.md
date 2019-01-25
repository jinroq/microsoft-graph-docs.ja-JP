---
title: ディレクトリの設定を取得します。
description: 特定のディレクトリの設定オブジェクトのプロパティを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ad7b0137e741ff6c6766980f121838ae00d8200
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525291"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="f4b34-103">ディレクトリの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="f4b34-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b34-104">特定のディレクトリの設定オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="f4b34-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="f4b34-105">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="f4b34-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f4b34-106">この API の/v1.0 バージョンの名前は*groupSettings を取得*します。</span><span class="sxs-lookup"><span data-stu-id="f4b34-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4b34-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f4b34-107">Permissions</span></span>
<span data-ttu-id="f4b34-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4b34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4b34-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4b34-110">Permission type</span></span>      | <span data-ttu-id="f4b34-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4b34-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4b34-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4b34-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4b34-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4b34-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4b34-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4b34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4b34-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4b34-115">Not supported.</span></span>    |
|<span data-ttu-id="f4b34-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4b34-116">Application</span></span> | <span data-ttu-id="f4b34-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b34-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4b34-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4b34-118">HTTP request</span></span>
<span data-ttu-id="f4b34-119"><!-- { "blockType": "ignored" } -->特定のテナント全体を取得または設定をグループ化</span><span class="sxs-lookup"><span data-stu-id="f4b34-119"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f4b34-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4b34-120">Optional query parameters</span></span>
<span data-ttu-id="f4b34-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4b34-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4b34-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4b34-122">Request headers</span></span>
| <span data-ttu-id="f4b34-123">名前</span><span class="sxs-lookup"><span data-stu-id="f4b34-123">Name</span></span>      |<span data-ttu-id="f4b34-124">説明</span><span class="sxs-lookup"><span data-stu-id="f4b34-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4b34-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4b34-125">Authorization</span></span>  | <span data-ttu-id="f4b34-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f4b34-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4b34-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4b34-128">Request body</span></span>
<span data-ttu-id="f4b34-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4b34-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4b34-130">応答</span><span class="sxs-lookup"><span data-stu-id="f4b34-130">Response</span></span>

<span data-ttu-id="f4b34-131">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[directorySetting](../resources/directorysetting.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f4b34-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4b34-132">例</span><span class="sxs-lookup"><span data-stu-id="f4b34-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4b34-133">要求</span><span class="sxs-lookup"><span data-stu-id="f4b34-133">Request</span></span>
<span data-ttu-id="f4b34-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4b34-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="f4b34-135">応答</span><span class="sxs-lookup"><span data-stu-id="f4b34-135">Response</span></span>
<span data-ttu-id="f4b34-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4b34-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
