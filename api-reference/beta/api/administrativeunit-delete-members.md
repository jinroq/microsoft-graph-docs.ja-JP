---
title: メンバーを削除する
description: この API を使用して、管理単位からメンバ (ユーザーまたはグループ) を削除します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9c605f9c77a715c8754edf3d83f7997e7cc4e865
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322988"
---
# <a name="remove-a-member"></a><span data-ttu-id="ed67f-103">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="ed67f-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed67f-104">この API を使用して、管理単位からメンバ (ユーザーまたはグループ) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ed67f-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed67f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed67f-105">Permissions</span></span>
<span data-ttu-id="ed67f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ed67f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed67f-108">Permission type</span></span>      | <span data-ttu-id="ed67f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed67f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed67f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed67f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed67f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed67f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed67f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed67f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed67f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed67f-113">Not supported.</span></span>    |
|<span data-ttu-id="ed67f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed67f-114">Application</span></span> | <span data-ttu-id="ed67f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed67f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed67f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed67f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ed67f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed67f-117">Request headers</span></span>
| <span data-ttu-id="ed67f-118">名前</span><span class="sxs-lookup"><span data-stu-id="ed67f-118">Name</span></span>      |<span data-ttu-id="ed67f-119">説明</span><span class="sxs-lookup"><span data-stu-id="ed67f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed67f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed67f-120">Authorization</span></span>  | <span data-ttu-id="ed67f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed67f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed67f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed67f-123">Request body</span></span>
<span data-ttu-id="ed67f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ed67f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed67f-125">応答</span><span class="sxs-lookup"><span data-stu-id="ed67f-125">Response</span></span>

<span data-ttu-id="ed67f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ed67f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed67f-128">例</span><span class="sxs-lookup"><span data-stu-id="ed67f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed67f-129">要求</span><span class="sxs-lookup"><span data-stu-id="ed67f-129">Request</span></span>
<span data-ttu-id="ed67f-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed67f-130">Here is an example of the request.</span></span> <span data-ttu-id="ed67f-131">次の例では、id1 はターゲット管理単位の識別子を表し、id2 は、targetted 管理単位から削除されるメンバーユーザーまたはグループの一意識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="ed67f-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="ed67f-132">応答</span><span class="sxs-lookup"><span data-stu-id="ed67f-132">Response</span></span>
<span data-ttu-id="ed67f-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ed67f-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
