---
title: RegisteredOwner を作成する
description: ユーザーをデバイスの登録済み所有者として追加します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 24c5c7977e8989bd4b790df3ec0629f61a654422
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528747"
---
# <a name="create-registeredowner"></a><span data-ttu-id="169b5-103">RegisteredOwner を作成する</span><span class="sxs-lookup"><span data-stu-id="169b5-103">Create registeredOwner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="169b5-104">ユーザーをデバイスの登録済み所有者として追加します。</span><span class="sxs-lookup"><span data-stu-id="169b5-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="169b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="169b5-105">Permissions</span></span>
<span data-ttu-id="169b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="169b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="169b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="169b5-108">Permission type</span></span>      | <span data-ttu-id="169b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="169b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="169b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="169b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="169b5-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="169b5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="169b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="169b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="169b5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="169b5-113">Not supported.</span></span>    |
|<span data-ttu-id="169b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="169b5-114">Application</span></span> | <span data-ttu-id="169b5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="169b5-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="169b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="169b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="169b5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="169b5-117">Request headers</span></span>
| <span data-ttu-id="169b5-118">名前</span><span class="sxs-lookup"><span data-stu-id="169b5-118">Name</span></span>       | <span data-ttu-id="169b5-119">型</span><span class="sxs-lookup"><span data-stu-id="169b5-119">Type</span></span> | <span data-ttu-id="169b5-120">説明</span><span class="sxs-lookup"><span data-stu-id="169b5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="169b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="169b5-121">Authorization</span></span>  | <span data-ttu-id="169b5-122">string</span><span class="sxs-lookup"><span data-stu-id="169b5-122">string</span></span>  | <span data-ttu-id="169b5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="169b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="169b5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="169b5-125">Request body</span></span>
<span data-ttu-id="169b5-126">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="169b5-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="169b5-127">応答</span><span class="sxs-lookup"><span data-stu-id="169b5-127">Response</span></span>

<span data-ttu-id="169b5-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="169b5-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="169b5-129">例</span><span class="sxs-lookup"><span data-stu-id="169b5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="169b5-130">要求</span><span class="sxs-lookup"><span data-stu-id="169b5-130">Request</span></span>
<span data-ttu-id="169b5-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="169b5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="169b5-132">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="169b5-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="169b5-133">応答</span><span class="sxs-lookup"><span data-stu-id="169b5-133">Response</span></span>
<span data-ttu-id="169b5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="169b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-post-registeredowners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
