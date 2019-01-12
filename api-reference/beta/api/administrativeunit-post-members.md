---
title: メンバーを追加する
description: 管理単位に (ユーザーまたはグループ) のメンバーを追加するのにはこの API を使用します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f64ca4c00265903fa1b4ebc467f2d70274628078
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946827"
---
# <a name="add-a-member"></a><span data-ttu-id="9aecd-103">メンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="9aecd-103">Add a member</span></span>

> <span data-ttu-id="9aecd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9aecd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aecd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9aecd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9aecd-106">管理単位に (ユーザーまたはグループ) のメンバーを追加するのにはこの API を使用します。</span><span class="sxs-lookup"><span data-stu-id="9aecd-106">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="9aecd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9aecd-107">Permissions</span></span>
<span data-ttu-id="9aecd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9aecd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9aecd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9aecd-110">Permission type</span></span>      | <span data-ttu-id="9aecd-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9aecd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9aecd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9aecd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9aecd-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9aecd-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9aecd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9aecd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9aecd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9aecd-115">Not supported.</span></span>    |
|<span data-ttu-id="9aecd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9aecd-116">Application</span></span> | <span data-ttu-id="9aecd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9aecd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9aecd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9aecd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9aecd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9aecd-119">Request headers</span></span>
| <span data-ttu-id="9aecd-120">名前</span><span class="sxs-lookup"><span data-stu-id="9aecd-120">Name</span></span>      |<span data-ttu-id="9aecd-121">説明</span><span class="sxs-lookup"><span data-stu-id="9aecd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9aecd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aecd-122">Authorization</span></span>  | <span data-ttu-id="9aecd-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9aecd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9aecd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9aecd-125">Request body</span></span>
<span data-ttu-id="9aecd-126">要求の本文に、[ユーザー](../resources/user.md)、[グループ](../resources/group.md)または追加するのには、 [directoryObject](../resources/directoryobject.md)の JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9aecd-126">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9aecd-127">応答</span><span class="sxs-lookup"><span data-stu-id="9aecd-127">Response</span></span>

<span data-ttu-id="9aecd-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9aecd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aecd-130">例</span><span class="sxs-lookup"><span data-stu-id="9aecd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9aecd-131">要求</span><span class="sxs-lookup"><span data-stu-id="9aecd-131">Request</span></span>
<span data-ttu-id="9aecd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9aecd-132">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="9aecd-133">要求の本文に指定の JSON 表現、`id`を追加する[ユーザー](../resources/user.md)または[グループ](../resources/group.md)のオブジェクトの。</span><span class="sxs-lookup"><span data-stu-id="9aecd-133">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="9aecd-134">応答</span><span class="sxs-lookup"><span data-stu-id="9aecd-134">Response</span></span>
<span data-ttu-id="9aecd-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="9aecd-135">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
