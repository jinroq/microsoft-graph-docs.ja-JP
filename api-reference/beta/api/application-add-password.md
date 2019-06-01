---
title: アプリケーションパスワードを追加する
description: アプリケーションに強力なパスワードを追加します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ee2000daba1f003705979ceb04e78ed920ea9281
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655160"
---
# <a name="add-application-password"></a><span data-ttu-id="5d599-103">アプリケーションパスワードを追加する</span><span class="sxs-lookup"><span data-stu-id="5d599-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d599-104">アプリケーションに強力なパスワードを追加します。</span><span class="sxs-lookup"><span data-stu-id="5d599-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d599-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d599-105">Permissions</span></span>
<span data-ttu-id="5d599-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d599-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d599-108">Permission type</span></span>      | <span data-ttu-id="5d599-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d599-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d599-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d599-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d599-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d599-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d599-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d599-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d599-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d599-113">Not supported.</span></span>    |
|<span data-ttu-id="5d599-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d599-114">Application</span></span> | <span data-ttu-id="5d599-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d599-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d599-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d599-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="5d599-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d599-117">Request headers</span></span>
| <span data-ttu-id="5d599-118">名前</span><span class="sxs-lookup"><span data-stu-id="5d599-118">Name</span></span>       | <span data-ttu-id="5d599-119">型</span><span class="sxs-lookup"><span data-stu-id="5d599-119">Type</span></span> | <span data-ttu-id="5d599-120">説明</span><span class="sxs-lookup"><span data-stu-id="5d599-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5d599-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d599-121">Authorization</span></span>  | <span data-ttu-id="5d599-122">string</span><span class="sxs-lookup"><span data-stu-id="5d599-122">string</span></span>  | <span data-ttu-id="5d599-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5d599-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d599-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d599-125">Request body</span></span>
<span data-ttu-id="5d599-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d599-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d599-127">応答</span><span class="sxs-lookup"><span data-stu-id="5d599-127">Response</span></span>

<span data-ttu-id="5d599-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で password オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5d599-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="5d599-129">Azure AD は、プロパティによって`secretText`返される強力なパスワードを生成します。</span><span class="sxs-lookup"><span data-stu-id="5d599-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="5d599-130">今後、このパスワードを取得する方法はありません。</span><span class="sxs-lookup"><span data-stu-id="5d599-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="5d599-131">例</span><span class="sxs-lookup"><span data-stu-id="5d599-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d599-132">要求</span><span class="sxs-lookup"><span data-stu-id="5d599-132">Request</span></span>
<span data-ttu-id="5d599-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5d599-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="5d599-134">応答</span><span class="sxs-lookup"><span data-stu-id="5d599-134">Response</span></span>
<span data-ttu-id="5d599-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5d599-135">Here is an example of the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "customKeyIdentifier": "Binary",
    "endDateTime": "String (timestamp)",
    "keyId": "String (identifier)",
    "startDateTime": "String (timestamp)",
    "secretText": "String",
    "hint": "String"
}
```
