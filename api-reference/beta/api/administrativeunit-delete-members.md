---
title: メンバーを削除する
description: 管理単位からメンバー (ユーザーまたはグループ) を削除するのにはこの API を使用します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e79dac5b7ae3a20675f6faaf9b209f8117ca2252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941528"
---
# <a name="remove-a-member"></a><span data-ttu-id="b4d6d-103">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="b4d6d-103">Remove a member</span></span>

> <span data-ttu-id="b4d6d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4d6d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4d6d-106">管理単位からメンバー (ユーザーまたはグループ) を削除するのにはこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-106">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4d6d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4d6d-107">Permissions</span></span>
<span data-ttu-id="b4d6d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b4d6d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4d6d-110">Permission type</span></span>      | <span data-ttu-id="b4d6d-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4d6d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4d6d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4d6d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b4d6d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4d6d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4d6d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4d6d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d6d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-115">Not supported.</span></span>    |
|<span data-ttu-id="b4d6d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4d6d-116">Application</span></span> | <span data-ttu-id="b4d6d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4d6d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4d6d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b4d6d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4d6d-119">Request headers</span></span>
| <span data-ttu-id="b4d6d-120">名前</span><span class="sxs-lookup"><span data-stu-id="b4d6d-120">Name</span></span>      |<span data-ttu-id="b4d6d-121">説明</span><span class="sxs-lookup"><span data-stu-id="b4d6d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4d6d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4d6d-122">Authorization</span></span>  | <span data-ttu-id="b4d6d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4d6d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4d6d-125">Request body</span></span>
<span data-ttu-id="b4d6d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d6d-127">応答</span><span class="sxs-lookup"><span data-stu-id="b4d6d-127">Response</span></span>

<span data-ttu-id="b4d6d-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4d6d-130">例</span><span class="sxs-lookup"><span data-stu-id="b4d6d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4d6d-131">要求</span><span class="sxs-lookup"><span data-stu-id="b4d6d-131">Request</span></span>
<span data-ttu-id="b4d6d-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-132">Here is an example of the request.</span></span> <span data-ttu-id="b4d6d-133">次の例では、id1 は、ターゲットの管理単位の id を表します、id2 属性は、対象の管理単位から削除するには、メンバー ユーザーまたはグループの一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-133">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="b4d6d-134">応答</span><span class="sxs-lookup"><span data-stu-id="b4d6d-134">Response</span></span>
<span data-ttu-id="b4d6d-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b4d6d-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
