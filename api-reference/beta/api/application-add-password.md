---
title: アプリケーションのパスワードを追加します。
description: 強力なパスワードをアプリケーションに追加します。
ms.openlocfilehash: 78ccb6cced055ca7f2d2ab201e844a9f50f36939
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067027"
---
# <a name="add-application-password"></a><span data-ttu-id="5b2a2-103">アプリケーションのパスワードを追加します。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-103">Add application password</span></span>

> <span data-ttu-id="5b2a2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b2a2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b2a2-106">強力なパスワードをアプリケーションに追加します。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b2a2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5b2a2-107">Permissions</span></span>
<span data-ttu-id="5b2a2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b2a2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b2a2-110">Permission type</span></span>      | <span data-ttu-id="5b2a2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b2a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b2a2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b2a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b2a2-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b2a2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b2a2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b2a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b2a2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-115">Not supported.</span></span>    |
|<span data-ttu-id="5b2a2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b2a2-116">Application</span></span> | <span data-ttu-id="5b2a2-117">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b2a2-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b2a2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b2a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="5b2a2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b2a2-119">Request headers</span></span>
| <span data-ttu-id="5b2a2-120">名前</span><span class="sxs-lookup"><span data-stu-id="5b2a2-120">Name</span></span>       | <span data-ttu-id="5b2a2-121">型</span><span class="sxs-lookup"><span data-stu-id="5b2a2-121">Type</span></span> | <span data-ttu-id="5b2a2-122">説明</span><span class="sxs-lookup"><span data-stu-id="5b2a2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b2a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b2a2-123">Authorization</span></span>  | <span data-ttu-id="5b2a2-124">string</span><span class="sxs-lookup"><span data-stu-id="5b2a2-124">string</span></span>  | <span data-ttu-id="5b2a2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5b2a2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b2a2-127">Request body</span></span>
<span data-ttu-id="5b2a2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b2a2-129">応答</span><span class="sxs-lookup"><span data-stu-id="5b2a2-129">Response</span></span>

<span data-ttu-id="5b2a2-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードとパスワードのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="5b2a2-131">Azure AD 経由で返されますが、強力なパスワードを生成する、`secretText`プロパティ。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="5b2a2-132">将来的にこのパスワードを取得する方法はありません。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="5b2a2-133">例</span><span class="sxs-lookup"><span data-stu-id="5b2a2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b2a2-134">要求</span><span class="sxs-lookup"><span data-stu-id="5b2a2-134">Request</span></span>
<span data-ttu-id="5b2a2-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="5b2a2-136">応答</span><span class="sxs-lookup"><span data-stu-id="5b2a2-136">Response</span></span>
<span data-ttu-id="5b2a2-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5b2a2-137">Here is an example of the response.</span></span>

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
