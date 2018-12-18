---
title: ディレクトリ設定は、グループを作成します。
description: グループの新しいディレクトリの設定を作成するのにには、この API を使用します。
author: dkershaw10
ms.openlocfilehash: 2e400babc809bdc8d9277cad1bd41b8b714e4e92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358997"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="889bb-103">ディレクトリ設定は、グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="889bb-103">Create a directory setting on groups</span></span>

> <span data-ttu-id="889bb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="889bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="889bb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="889bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="889bb-106">グループの新しいディレクトリの設定を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="889bb-106">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="889bb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="889bb-107">Permissions</span></span>
<span data-ttu-id="889bb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="889bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="889bb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="889bb-110">Permission type</span></span>      | <span data-ttu-id="889bb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="889bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="889bb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="889bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="889bb-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="889bb-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="889bb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="889bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="889bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="889bb-115">Not supported.</span></span>    |
|<span data-ttu-id="889bb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="889bb-116">Application</span></span> | <span data-ttu-id="889bb-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="889bb-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="889bb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="889bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="889bb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="889bb-119">Request headers</span></span>
| <span data-ttu-id="889bb-120">名前</span><span class="sxs-lookup"><span data-stu-id="889bb-120">Name</span></span>       | <span data-ttu-id="889bb-121">説明</span><span class="sxs-lookup"><span data-stu-id="889bb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="889bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="889bb-122">Authorization</span></span>  | <span data-ttu-id="889bb-123">ベアラー <token>。</span><span class="sxs-lookup"><span data-stu-id="889bb-123">Bearer <token>.</span></span> <span data-ttu-id="889bb-124">必須</span><span class="sxs-lookup"><span data-stu-id="889bb-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="889bb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="889bb-125">Request body</span></span>
<span data-ttu-id="889bb-126">要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="889bb-126">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="889bb-127">応答</span><span class="sxs-lookup"><span data-stu-id="889bb-127">Response</span></span>

<span data-ttu-id="889bb-128">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[directorySetting](../resources/directorysetting.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="889bb-128">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="889bb-129">例</span><span class="sxs-lookup"><span data-stu-id="889bb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="889bb-130">要求</span><span class="sxs-lookup"><span data-stu-id="889bb-130">Request</span></span>
<span data-ttu-id="889bb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="889bb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="889bb-132">要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="889bb-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="889bb-133">応答</span><span class="sxs-lookup"><span data-stu-id="889bb-133">Response</span></span>
<span data-ttu-id="889bb-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="889bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->