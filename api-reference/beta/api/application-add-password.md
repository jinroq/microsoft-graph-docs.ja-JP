---
title: アプリケーションのパスワードを追加します。
description: 強力なパスワードをアプリケーションに追加します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 15189ee709b2b369d014f9854bcdbd4dc1b7e9be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526824"
---
# <a name="add-application-password"></a><span data-ttu-id="03def-103">アプリケーションのパスワードを追加します。</span><span class="sxs-lookup"><span data-stu-id="03def-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03def-104">強力なパスワードをアプリケーションに追加します。</span><span class="sxs-lookup"><span data-stu-id="03def-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="03def-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03def-105">Permissions</span></span>
<span data-ttu-id="03def-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03def-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03def-108">Permission type</span></span>      | <span data-ttu-id="03def-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03def-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03def-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03def-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03def-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03def-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03def-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03def-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03def-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03def-113">Not supported.</span></span>    |
|<span data-ttu-id="03def-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03def-114">Application</span></span> | <span data-ttu-id="03def-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="03def-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03def-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03def-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="03def-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03def-117">Request headers</span></span>
| <span data-ttu-id="03def-118">名前</span><span class="sxs-lookup"><span data-stu-id="03def-118">Name</span></span>       | <span data-ttu-id="03def-119">型</span><span class="sxs-lookup"><span data-stu-id="03def-119">Type</span></span> | <span data-ttu-id="03def-120">説明</span><span class="sxs-lookup"><span data-stu-id="03def-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="03def-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03def-121">Authorization</span></span>  | <span data-ttu-id="03def-122">string</span><span class="sxs-lookup"><span data-stu-id="03def-122">string</span></span>  | <span data-ttu-id="03def-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03def-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03def-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="03def-125">Request body</span></span>
<span data-ttu-id="03def-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="03def-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03def-127">応答</span><span class="sxs-lookup"><span data-stu-id="03def-127">Response</span></span>

<span data-ttu-id="03def-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードとパスワードのオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="03def-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="03def-129">Azure AD 経由で返されますが、強力なパスワードを生成する、`secretText`プロパティ。</span><span class="sxs-lookup"><span data-stu-id="03def-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="03def-130">将来的にこのパスワードを取得する方法はありません。</span><span class="sxs-lookup"><span data-stu-id="03def-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="03def-131">例</span><span class="sxs-lookup"><span data-stu-id="03def-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03def-132">要求</span><span class="sxs-lookup"><span data-stu-id="03def-132">Request</span></span>
<span data-ttu-id="03def-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03def-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="03def-134">応答</span><span class="sxs-lookup"><span data-stu-id="03def-134">Response</span></span>
<span data-ttu-id="03def-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="03def-135">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/application-add-password.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
