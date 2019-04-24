---
title: グループにディレクトリ設定を作成する
description: この API を使用して、グループの新しいディレクトリ設定を作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3ba33de148e34ce80c0a709a6a1b5faf99d5f32d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502095"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="3237a-103">グループにディレクトリ設定を作成する</span><span class="sxs-lookup"><span data-stu-id="3237a-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3237a-104">この API を使用して、グループの新しいディレクトリ設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="3237a-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="3237a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3237a-105">Permissions</span></span>
<span data-ttu-id="3237a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3237a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3237a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3237a-108">Permission type</span></span>      | <span data-ttu-id="3237a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3237a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3237a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3237a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3237a-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3237a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3237a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3237a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3237a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3237a-113">Not supported.</span></span>    |
|<span data-ttu-id="3237a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3237a-114">Application</span></span> | <span data-ttu-id="3237a-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3237a-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3237a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3237a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="3237a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3237a-117">Request headers</span></span>
| <span data-ttu-id="3237a-118">名前</span><span class="sxs-lookup"><span data-stu-id="3237a-118">Name</span></span>       | <span data-ttu-id="3237a-119">説明</span><span class="sxs-lookup"><span data-stu-id="3237a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3237a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3237a-120">Authorization</span></span>  | <span data-ttu-id="3237a-121">ベアラー <token>。</span><span class="sxs-lookup"><span data-stu-id="3237a-121">Bearer <token>.</span></span> <span data-ttu-id="3237a-122">必須</span><span class="sxs-lookup"><span data-stu-id="3237a-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3237a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3237a-123">Request body</span></span>
<span data-ttu-id="3237a-124">要求本文で、 [directorysetting](../resources/directorysetting.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3237a-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3237a-125">応答</span><span class="sxs-lookup"><span data-stu-id="3237a-125">Response</span></span>

<span data-ttu-id="3237a-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[directorysetting](../resources/directorysetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3237a-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3237a-127">例</span><span class="sxs-lookup"><span data-stu-id="3237a-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3237a-128">要求</span><span class="sxs-lookup"><span data-stu-id="3237a-128">Request</span></span>
<span data-ttu-id="3237a-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3237a-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="3237a-130">要求本文で、 [directorysetting](../resources/directorysetting.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3237a-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3237a-131">応答</span><span class="sxs-lookup"><span data-stu-id="3237a-131">Response</span></span>
<span data-ttu-id="3237a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3237a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
