---
title: ディレクトリ設定は、グループを作成します。
description: グループの新しいディレクトリの設定を作成するのにには、この API を使用します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3ba33de148e34ce80c0a709a6a1b5faf99d5f32d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515847"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="f6533-103">ディレクトリ設定は、グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6533-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6533-104">グループの新しいディレクトリの設定を作成するのにには、この API を使用します。</span><span class="sxs-lookup"><span data-stu-id="f6533-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6533-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6533-105">Permissions</span></span>
<span data-ttu-id="f6533-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6533-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6533-108">Permission type</span></span>      | <span data-ttu-id="f6533-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6533-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6533-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6533-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6533-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6533-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6533-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6533-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6533-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6533-113">Not supported.</span></span>    |
|<span data-ttu-id="f6533-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6533-114">Application</span></span> | <span data-ttu-id="f6533-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6533-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6533-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6533-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="f6533-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6533-117">Request headers</span></span>
| <span data-ttu-id="f6533-118">名前</span><span class="sxs-lookup"><span data-stu-id="f6533-118">Name</span></span>       | <span data-ttu-id="f6533-119">説明</span><span class="sxs-lookup"><span data-stu-id="f6533-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f6533-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6533-120">Authorization</span></span>  | <span data-ttu-id="f6533-121">ベアラー <token>。</span><span class="sxs-lookup"><span data-stu-id="f6533-121">Bearer <token>.</span></span> <span data-ttu-id="f6533-122">必須</span><span class="sxs-lookup"><span data-stu-id="f6533-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6533-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6533-123">Request body</span></span>
<span data-ttu-id="f6533-124">要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6533-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f6533-125">応答</span><span class="sxs-lookup"><span data-stu-id="f6533-125">Response</span></span>

<span data-ttu-id="f6533-126">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[directorySetting](../resources/directorysetting.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f6533-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6533-127">例</span><span class="sxs-lookup"><span data-stu-id="f6533-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6533-128">要求</span><span class="sxs-lookup"><span data-stu-id="f6533-128">Request</span></span>
<span data-ttu-id="f6533-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6533-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="f6533-130">要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6533-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f6533-131">応答</span><span class="sxs-lookup"><span data-stu-id="f6533-131">Response</span></span>
<span data-ttu-id="f6533-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6533-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
