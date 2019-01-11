---
title: 'ユーザー: exportPersonalData'
description: 組織のユーザーのデータをエクスポートするのには企業の管理者によって行われる、データ ポリシーの操作要求を送信します。
localization_priority: Normal
ms.openlocfilehash: d660994868e331fb8c1813bb9ff90aebe4790e9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845340"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="268bc-103">ユーザー: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="268bc-103">user: exportPersonalData</span></span>

<span data-ttu-id="268bc-104">組織のユーザーのデータをエクスポートするのには、企業の管理者によって行われた、データ ポリシーの操作要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="268bc-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="268bc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="268bc-105">Permissions</span></span>
<span data-ttu-id="268bc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="268bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="268bc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="268bc-108">Permission type</span></span>      | <span data-ttu-id="268bc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="268bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="268bc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="268bc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="268bc-111">User.Export.All と User.Read.All</span><span class="sxs-lookup"><span data-stu-id="268bc-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="268bc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="268bc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="268bc-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="268bc-113">Not applicable</span></span>  |
|<span data-ttu-id="268bc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="268bc-114">Application</span></span> | <span data-ttu-id="268bc-115">User.Export.All と User.Read.All</span><span class="sxs-lookup"><span data-stu-id="268bc-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="268bc-116">**注:** エクスポートだけは企業の管理者、委任されたアクセス許可を使用するとします。</span><span class="sxs-lookup"><span data-stu-id="268bc-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="268bc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="268bc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="268bc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="268bc-118">Request headers</span></span>
| <span data-ttu-id="268bc-119">名前</span><span class="sxs-lookup"><span data-stu-id="268bc-119">Name</span></span>       | <span data-ttu-id="268bc-120">説明</span><span class="sxs-lookup"><span data-stu-id="268bc-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="268bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="268bc-121">Authorization</span></span>  | <span data-ttu-id="268bc-122">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="268bc-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="268bc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="268bc-123">Request body</span></span>
<span data-ttu-id="268bc-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="268bc-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="268bc-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="268bc-125">Parameter</span></span>    | <span data-ttu-id="268bc-126">Type</span><span class="sxs-lookup"><span data-stu-id="268bc-126">Type</span></span>   |<span data-ttu-id="268bc-127">説明</span><span class="sxs-lookup"><span data-stu-id="268bc-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="268bc-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="268bc-128">storageLocation</span></span>|<span data-ttu-id="268bc-129">String</span><span class="sxs-lookup"><span data-stu-id="268bc-129">String</span></span>|<span data-ttu-id="268bc-130">これは、データをエクスポートする必要があります、Azure ストレージ アカウントに共有アクセス署名 (SA) の URL です。</span><span class="sxs-lookup"><span data-stu-id="268bc-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="268bc-131">応答</span><span class="sxs-lookup"><span data-stu-id="268bc-131">Response</span></span>
<span data-ttu-id="268bc-132">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="268bc-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="268bc-133">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="268bc-133">It does not return anything in the response body.</span></span> <span data-ttu-id="268bc-134">応答には、次のヘッダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="268bc-134">The response contains the following headers.</span></span>

| <span data-ttu-id="268bc-135">名前</span><span class="sxs-lookup"><span data-stu-id="268bc-135">Name</span></span>       | <span data-ttu-id="268bc-136">説明</span><span class="sxs-lookup"><span data-stu-id="268bc-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="268bc-137">Location</span><span class="sxs-lookup"><span data-stu-id="268bc-137">Location</span></span>  | <span data-ttu-id="268bc-138">要求のステータスを確認する URL です。</span><span class="sxs-lookup"><span data-stu-id="268bc-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="268bc-139">再試行した後</span><span class="sxs-lookup"><span data-stu-id="268bc-139">Retry-After</span></span>  | <span data-ttu-id="268bc-140">までの時間 (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="268bc-140">Time period in seconds.</span></span> <span data-ttu-id="268bc-141">要求のメーカーは、これを待つ必要があります後の状態をチェックする要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="268bc-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="268bc-142">例</span><span class="sxs-lookup"><span data-stu-id="268bc-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="268bc-143">要求</span><span class="sxs-lookup"><span data-stu-id="268bc-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="268bc-144">応答</span><span class="sxs-lookup"><span data-stu-id="268bc-144">Response</span></span>

```
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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
  "tocPath": ""
}-->
