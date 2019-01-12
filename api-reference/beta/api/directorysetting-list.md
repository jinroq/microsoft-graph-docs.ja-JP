---
title: リストのディレクトリの設定
description: ディレクトリ オブジェクトの設定の一覧を取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 651d8588c416d25dd20ac07a36ac3ca30f1b334e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985271"
---
# <a name="list-directory-settings"></a><span data-ttu-id="5ef91-103">リストのディレクトリの設定</span><span class="sxs-lookup"><span data-stu-id="5ef91-103">List directory settings</span></span>

> <span data-ttu-id="5ef91-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ef91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ef91-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ef91-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ef91-106">ディレクトリ オブジェクトの設定の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5ef91-106">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="5ef91-107">**注**: この API の/beta バージョンは、のみのグループに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5ef91-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="5ef91-108">この API の/v1.0 のバージョンは*groupSettings のリスト*に名前変更されました。</span><span class="sxs-lookup"><span data-stu-id="5ef91-108">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ef91-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ef91-109">Permissions</span></span>
<span data-ttu-id="5ef91-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ef91-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef91-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ef91-112">Permission type</span></span>      | <span data-ttu-id="5ef91-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ef91-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ef91-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ef91-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5ef91-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ef91-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ef91-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ef91-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ef91-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ef91-117">Not supported.</span></span>    |
|<span data-ttu-id="5ef91-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ef91-118">Application</span></span> | <span data-ttu-id="5ef91-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ef91-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ef91-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ef91-120">HTTP request</span></span>
<span data-ttu-id="5ef91-121"><!-- { "blockType": "ignored" } -->テナント全体を一覧表示またはグループの設定</span><span class="sxs-lookup"><span data-stu-id="5ef91-121"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ef91-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5ef91-122">Optional query parameters</span></span>
<span data-ttu-id="5ef91-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5ef91-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ef91-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ef91-124">Request headers</span></span>
| <span data-ttu-id="5ef91-125">名前</span><span class="sxs-lookup"><span data-stu-id="5ef91-125">Name</span></span>      |<span data-ttu-id="5ef91-126">説明</span><span class="sxs-lookup"><span data-stu-id="5ef91-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ef91-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ef91-127">Authorization</span></span>  | <span data-ttu-id="5ef91-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ef91-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ef91-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ef91-130">Request body</span></span>
<span data-ttu-id="5ef91-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ef91-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ef91-132">応答</span><span class="sxs-lookup"><span data-stu-id="5ef91-132">Response</span></span>

<span data-ttu-id="5ef91-133">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[directorySetting](../resources/directorysetting.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5ef91-133">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ef91-134">例</span><span class="sxs-lookup"><span data-stu-id="5ef91-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ef91-135">要求</span><span class="sxs-lookup"><span data-stu-id="5ef91-135">Request</span></span>
<span data-ttu-id="5ef91-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ef91-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="5ef91-137">応答</span><span class="sxs-lookup"><span data-stu-id="5ef91-137">Response</span></span>
<span data-ttu-id="5ef91-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ef91-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
