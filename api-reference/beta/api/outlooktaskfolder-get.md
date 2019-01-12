---
title: OutlookTaskFolder を取得します。
description: プロパティと指定した Outlook の仕事フォルダーの関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7e8f8e9c1fa16b5e0a00b0f779d652d2c6e1aa93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929222"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="d5060-103">OutlookTaskFolder を取得します。</span><span class="sxs-lookup"><span data-stu-id="d5060-103">Get outlookTaskFolder</span></span>

> <span data-ttu-id="d5060-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5060-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5060-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5060-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5060-106">プロパティと指定した Outlook の仕事フォルダーの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="d5060-106">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5060-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5060-107">Permissions</span></span>
<span data-ttu-id="d5060-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5060-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5060-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5060-110">Permission type</span></span>      | <span data-ttu-id="d5060-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5060-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5060-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5060-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5060-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d5060-113">Tasks.Read</span></span>    |
|<span data-ttu-id="d5060-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5060-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5060-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d5060-115">Tasks.Read</span></span>    |
|<span data-ttu-id="d5060-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5060-116">Application</span></span> | <span data-ttu-id="d5060-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5060-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5060-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5060-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5060-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d5060-119">Optional query parameters</span></span>
<span data-ttu-id="d5060-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d5060-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5060-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5060-121">Request headers</span></span>
| <span data-ttu-id="d5060-122">名前</span><span class="sxs-lookup"><span data-stu-id="d5060-122">Name</span></span>      |<span data-ttu-id="d5060-123">説明</span><span class="sxs-lookup"><span data-stu-id="d5060-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5060-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5060-124">Authorization</span></span>  | <span data-ttu-id="d5060-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5060-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5060-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5060-127">Request body</span></span>
<span data-ttu-id="d5060-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d5060-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5060-129">応答</span><span class="sxs-lookup"><span data-stu-id="d5060-129">Response</span></span>

<span data-ttu-id="d5060-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[outlookTaskFolder](../resources/outlooktaskfolder.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d5060-130">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5060-131">例</span><span class="sxs-lookup"><span data-stu-id="d5060-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5060-132">要求</span><span class="sxs-lookup"><span data-stu-id="d5060-132">Request</span></span>
<span data-ttu-id="d5060-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5060-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAAABrJAAA=')
```
##### <a name="response"></a><span data-ttu-id="d5060-134">応答</span><span class="sxs-lookup"><span data-stu-id="d5060-134">Response</span></span>
<span data-ttu-id="d5060-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5060-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
