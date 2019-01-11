---
title: Outlook カテゴリを作成する
description: ユーザーのマスター カテゴリ リスト内に outlookCategory オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 4f032bff358fbc3c07b30f925abee27664c01c8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807092"
---
# <a name="create-outlook-category"></a><span data-ttu-id="a33e3-103">Outlook カテゴリを作成する</span><span class="sxs-lookup"><span data-stu-id="a33e3-103">Create Outlook category</span></span>

> <span data-ttu-id="a33e3-104">**重要**: [Microsoft Graph で/beta のバージョンの Api を選択し、プレビューでは、変更されることができます。</span><span class="sxs-lookup"><span data-stu-id="a33e3-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a33e3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a33e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a33e3-106">ユーザーのマスター カテゴリ リスト内に [outlookCategory](../resources/outlookcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a33e3-106">Create an [outlookCategory](../resources/outlookcategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="a33e3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a33e3-107">Permissions</span></span>
<span data-ttu-id="a33e3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a33e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a33e3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a33e3-110">Permission type</span></span>      | <span data-ttu-id="a33e3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a33e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a33e3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a33e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a33e3-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a33e3-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a33e3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a33e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a33e3-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a33e3-115">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="a33e3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a33e3-116">Application</span></span> | <span data-ttu-id="a33e3-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a33e3-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a33e3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a33e3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="a33e3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a33e3-119">Request headers</span></span>
| <span data-ttu-id="a33e3-120">名前</span><span class="sxs-lookup"><span data-stu-id="a33e3-120">Name</span></span>       | <span data-ttu-id="a33e3-121">説明</span><span class="sxs-lookup"><span data-stu-id="a33e3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a33e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a33e3-122">Authorization</span></span>  | <span data-ttu-id="a33e3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a33e3-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a33e3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a33e3-125">Request body</span></span>
<span data-ttu-id="a33e3-126">要求本文に、[outlookCategory](../resources/outlookcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a33e3-126">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a33e3-127">応答</span><span class="sxs-lookup"><span data-stu-id="a33e3-127">Response</span></span>

<span data-ttu-id="a33e3-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に [outlookCategory](../resources/outlookcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a33e3-128">If successful, this method returns `201 Created` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a33e3-129">例</span><span class="sxs-lookup"><span data-stu-id="a33e3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a33e3-130">要求</span><span class="sxs-lookup"><span data-stu-id="a33e3-130">Request</span></span>
<span data-ttu-id="a33e3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a33e3-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="a33e3-132">要求本文に、[outlookCategory](../resources/outlookcategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a33e3-132">In the request body, supply a JSON representation of [outlookCategory](../resources/outlookcategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a33e3-133">応答</span><span class="sxs-lookup"><span data-stu-id="a33e3-133">Response</span></span>
<span data-ttu-id="a33e3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a33e3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
