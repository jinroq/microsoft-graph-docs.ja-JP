---
title: メンバーを削除する
description: この API を使用して、管理単位からメンバ (ユーザーまたはグループ) を削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c307a802e2d574950b89c3f5644b5fbf70d90e34
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917934"
---
# <a name="remove-a-member"></a><span data-ttu-id="6b98a-103">メンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="6b98a-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b98a-104">この API を使用して、管理単位からメンバ (ユーザーまたはグループ) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6b98a-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b98a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6b98a-105">Permissions</span></span>
<span data-ttu-id="6b98a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b98a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6b98a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b98a-108">Permission type</span></span>      | <span data-ttu-id="6b98a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b98a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b98a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b98a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b98a-111">AdministrativeUnit。すべての Directory.accessasuser.all について</span><span class="sxs-lookup"><span data-stu-id="6b98a-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b98a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b98a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b98a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b98a-113">Not supported.</span></span>    |
|<span data-ttu-id="6b98a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b98a-114">Application</span></span> | <span data-ttu-id="6b98a-115">AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="6b98a-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b98a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b98a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6b98a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b98a-117">Request headers</span></span>
| <span data-ttu-id="6b98a-118">名前</span><span class="sxs-lookup"><span data-stu-id="6b98a-118">Name</span></span>      |<span data-ttu-id="6b98a-119">説明</span><span class="sxs-lookup"><span data-stu-id="6b98a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b98a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b98a-120">Authorization</span></span>  | <span data-ttu-id="6b98a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6b98a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b98a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b98a-123">Request body</span></span>
<span data-ttu-id="6b98a-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6b98a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b98a-125">応答</span><span class="sxs-lookup"><span data-stu-id="6b98a-125">Response</span></span>

<span data-ttu-id="6b98a-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6b98a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b98a-128">例</span><span class="sxs-lookup"><span data-stu-id="6b98a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b98a-129">要求</span><span class="sxs-lookup"><span data-stu-id="6b98a-129">Request</span></span>
<span data-ttu-id="6b98a-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b98a-130">Here is an example of the request.</span></span> <span data-ttu-id="6b98a-131">次の例では、id1 はターゲット管理単位の識別子を表し、id2 は、targetted 管理単位から削除されるメンバーユーザーまたはグループの一意識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6b98a-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="6b98a-132">応答</span><span class="sxs-lookup"><span data-stu-id="6b98a-132">Response</span></span>
<span data-ttu-id="6b98a-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6b98a-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
