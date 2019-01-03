---
title: RegisteredOwner を作成する
description: ユーザーをデバイスの登録済み所有者として追加します。
author: tfitzmac
ms.openlocfilehash: 39cbd53b634b3f1388a27acf81e80ca2a7953693
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342561"
---
# <a name="create-registeredowner"></a><span data-ttu-id="12ca0-103">RegisteredOwner を作成する</span><span class="sxs-lookup"><span data-stu-id="12ca0-103">Create registeredOwner</span></span>

> <span data-ttu-id="12ca0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="12ca0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12ca0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12ca0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12ca0-106">ユーザーをデバイスの登録済み所有者として追加します。</span><span class="sxs-lookup"><span data-stu-id="12ca0-106">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="12ca0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12ca0-107">Permissions</span></span>
<span data-ttu-id="12ca0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12ca0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12ca0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12ca0-110">Permission type</span></span>      | <span data-ttu-id="12ca0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="12ca0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12ca0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12ca0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12ca0-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12ca0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12ca0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12ca0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12ca0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12ca0-115">Not supported.</span></span>    |
|<span data-ttu-id="12ca0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12ca0-116">Application</span></span> | <span data-ttu-id="12ca0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12ca0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12ca0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12ca0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="12ca0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12ca0-119">Request headers</span></span>
| <span data-ttu-id="12ca0-120">名前</span><span class="sxs-lookup"><span data-stu-id="12ca0-120">Name</span></span>       | <span data-ttu-id="12ca0-121">種類</span><span class="sxs-lookup"><span data-stu-id="12ca0-121">Type</span></span> | <span data-ttu-id="12ca0-122">説明</span><span class="sxs-lookup"><span data-stu-id="12ca0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12ca0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12ca0-123">Authorization</span></span>  | <span data-ttu-id="12ca0-124">string</span><span class="sxs-lookup"><span data-stu-id="12ca0-124">string</span></span>  | <span data-ttu-id="12ca0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="12ca0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12ca0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="12ca0-127">Request body</span></span>
<span data-ttu-id="12ca0-128">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12ca0-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12ca0-129">応答</span><span class="sxs-lookup"><span data-stu-id="12ca0-129">Response</span></span>

<span data-ttu-id="12ca0-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12ca0-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12ca0-131">例</span><span class="sxs-lookup"><span data-stu-id="12ca0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12ca0-132">要求</span><span class="sxs-lookup"><span data-stu-id="12ca0-132">Request</span></span>
<span data-ttu-id="12ca0-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12ca0-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="12ca0-134">要求本文で、[directoryObject](../resources/directoryobject.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12ca0-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="12ca0-135">応答</span><span class="sxs-lookup"><span data-stu-id="12ca0-135">Response</span></span>
<span data-ttu-id="12ca0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12ca0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->