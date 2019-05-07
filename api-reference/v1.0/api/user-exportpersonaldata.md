---
title: 'ユーザー: Exportpersonal Data'
description: 組織のユーザーのデータをエクスポートするために、会社の管理者によって行われたデータポリシー操作要求を送信します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6feffbe56a6b4fe21c5a06eb89016f68d8f045ef
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602150"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="236bb-103">ユーザー: Exportpersonal Data</span><span class="sxs-lookup"><span data-stu-id="236bb-103">user: exportPersonalData</span></span>

<span data-ttu-id="236bb-104">組織のユーザーのデータをエクスポートするために、会社の管理者またはアプリケーションからデータポリシー操作要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="236bb-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="236bb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="236bb-105">Permissions</span></span>
<span data-ttu-id="236bb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="236bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="236bb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="236bb-108">Permission type</span></span>      | <span data-ttu-id="236bb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="236bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="236bb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="236bb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="236bb-111">すべてのユーザーをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="236bb-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="236bb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="236bb-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="236bb-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="236bb-113">Not applicable</span></span>  |
|<span data-ttu-id="236bb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="236bb-114">Application</span></span> | <span data-ttu-id="236bb-115">すべてのユーザーをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="236bb-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="236bb-116">**注:** エクスポートは、委任されたアクセス許可を使用する場合にのみ、会社の管理者が実行できます。</span><span class="sxs-lookup"><span data-stu-id="236bb-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="236bb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="236bb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="236bb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="236bb-118">Request headers</span></span>
| <span data-ttu-id="236bb-119">名前</span><span class="sxs-lookup"><span data-stu-id="236bb-119">Name</span></span>       | <span data-ttu-id="236bb-120">説明</span><span class="sxs-lookup"><span data-stu-id="236bb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="236bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="236bb-121">Authorization</span></span>  | <span data-ttu-id="236bb-122">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="236bb-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="236bb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="236bb-123">Request body</span></span>
<span data-ttu-id="236bb-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="236bb-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="236bb-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="236bb-125">Parameter</span></span>    | <span data-ttu-id="236bb-126">型</span><span class="sxs-lookup"><span data-stu-id="236bb-126">Type</span></span>   |<span data-ttu-id="236bb-127">説明</span><span class="sxs-lookup"><span data-stu-id="236bb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="236bb-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="236bb-128">storageLocation</span></span>|<span data-ttu-id="236bb-129">String</span><span class="sxs-lookup"><span data-stu-id="236bb-129">String</span></span>|<span data-ttu-id="236bb-130">これは、データのエクスポート先となる Azure Storage アカウントの shared access signature (SAS) URL です。</span><span class="sxs-lookup"><span data-stu-id="236bb-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="236bb-131">応答</span><span class="sxs-lookup"><span data-stu-id="236bb-131">Response</span></span>
<span data-ttu-id="236bb-132">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="236bb-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="236bb-133">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="236bb-133">It does not return anything in the response body.</span></span> <span data-ttu-id="236bb-134">応答には、次の応答ヘッダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="236bb-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="236bb-135">名前</span><span class="sxs-lookup"><span data-stu-id="236bb-135">Name</span></span>       | <span data-ttu-id="236bb-136">説明</span><span class="sxs-lookup"><span data-stu-id="236bb-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="236bb-137">Location</span><span class="sxs-lookup"><span data-stu-id="236bb-137">Location</span></span>  | <span data-ttu-id="236bb-138">要求の状態を確認するための URL。</span><span class="sxs-lookup"><span data-stu-id="236bb-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="236bb-139">再試行-後</span><span class="sxs-lookup"><span data-stu-id="236bb-139">Retry-After</span></span>  | <span data-ttu-id="236bb-140">期間 (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="236bb-140">Time period in seconds.</span></span> <span data-ttu-id="236bb-141">要求を送信した後に、要求の状態を確認するための要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="236bb-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="236bb-142">例</span><span class="sxs-lookup"><span data-stu-id="236bb-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="236bb-143">要求</span><span class="sxs-lookup"><span data-stu-id="236bb-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="236bb-144">応答</span><span class="sxs-lookup"><span data-stu-id="236bb-144">Response</span></span>

```
#### SDK sample code
# [C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Cs-snippets.md)]

# [Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
