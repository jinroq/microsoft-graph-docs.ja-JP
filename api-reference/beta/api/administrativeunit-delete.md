---
title: administrativeUnit の削除
description: administrativeUnit を削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bd325490e84266b11d8bb17463fa9f7e01547cf8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322828"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="d04ab-103">administrativeUnit の削除</span><span class="sxs-lookup"><span data-stu-id="d04ab-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d04ab-104">[administrativeUnit](../resources/administrativeunit.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d04ab-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d04ab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d04ab-105">Permissions</span></span>
<span data-ttu-id="d04ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d04ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d04ab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d04ab-108">Permission type</span></span>      | <span data-ttu-id="d04ab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d04ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d04ab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d04ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d04ab-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d04ab-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d04ab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d04ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d04ab-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d04ab-113">Not supported.</span></span>    |
|<span data-ttu-id="d04ab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d04ab-114">Application</span></span> | <span data-ttu-id="d04ab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d04ab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d04ab-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d04ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d04ab-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d04ab-117">Request headers</span></span>
| <span data-ttu-id="d04ab-118">名前</span><span class="sxs-lookup"><span data-stu-id="d04ab-118">Name</span></span>       | <span data-ttu-id="d04ab-119">説明</span><span class="sxs-lookup"><span data-stu-id="d04ab-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d04ab-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d04ab-120">Authorization</span></span>  | <span data-ttu-id="d04ab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d04ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d04ab-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d04ab-123">Request body</span></span>
<span data-ttu-id="d04ab-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d04ab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d04ab-125">応答</span><span class="sxs-lookup"><span data-stu-id="d04ab-125">Response</span></span>

<span data-ttu-id="d04ab-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d04ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d04ab-128">例</span><span class="sxs-lookup"><span data-stu-id="d04ab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d04ab-129">要求</span><span class="sxs-lookup"><span data-stu-id="d04ab-129">Request</span></span>
<span data-ttu-id="d04ab-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d04ab-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="d04ab-131">応答</span><span class="sxs-lookup"><span data-stu-id="d04ab-131">Response</span></span>
<span data-ttu-id="d04ab-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d04ab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
