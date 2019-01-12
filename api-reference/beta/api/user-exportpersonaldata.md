---
title: 'ユーザー: exportPersonalData'
description: 組織のユーザーのデータをエクスポートするのには企業の管理者によって行われる、データ ポリシーの操作要求を送信します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f112d065b75da7dc525e667df78b0264be37d55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934192"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="bcac9-103">ユーザー: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="bcac9-103">user: exportPersonalData</span></span>

<span data-ttu-id="bcac9-104">組織のユーザーのデータをエクスポートするのには、企業の管理者によって行われた、データ ポリシーの操作要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="bcac9-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcac9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bcac9-105">Permissions</span></span>
<span data-ttu-id="bcac9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcac9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bcac9-108">Permission type</span></span>      | <span data-ttu-id="bcac9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bcac9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcac9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bcac9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bcac9-111">User.Export.All と User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcac9-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="bcac9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bcac9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bcac9-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="bcac9-113">Not applicable</span></span>  |
|<span data-ttu-id="bcac9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bcac9-114">Application</span></span> | <span data-ttu-id="bcac9-115">User.Export.All と User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcac9-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="bcac9-116">**注:** エクスポートだけは企業の管理者、委任されたアクセス許可を使用するとします。</span><span class="sxs-lookup"><span data-stu-id="bcac9-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="bcac9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bcac9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="bcac9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcac9-118">Request headers</span></span>
| <span data-ttu-id="bcac9-119">名前</span><span class="sxs-lookup"><span data-stu-id="bcac9-119">Name</span></span>       | <span data-ttu-id="bcac9-120">説明</span><span class="sxs-lookup"><span data-stu-id="bcac9-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bcac9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcac9-121">Authorization</span></span>  | <span data-ttu-id="bcac9-122">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="bcac9-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcac9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bcac9-123">Request body</span></span>
<span data-ttu-id="bcac9-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bcac9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bcac9-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bcac9-125">Parameter</span></span>    | <span data-ttu-id="bcac9-126">Type</span><span class="sxs-lookup"><span data-stu-id="bcac9-126">Type</span></span>   |<span data-ttu-id="bcac9-127">説明</span><span class="sxs-lookup"><span data-stu-id="bcac9-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bcac9-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="bcac9-128">storageLocation</span></span>|<span data-ttu-id="bcac9-129">String</span><span class="sxs-lookup"><span data-stu-id="bcac9-129">String</span></span>|<span data-ttu-id="bcac9-130">これは、データをエクスポートする必要があります、Azure ストレージ アカウントに共有アクセス署名 (SA) の URL です。</span><span class="sxs-lookup"><span data-stu-id="bcac9-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="bcac9-131">応答</span><span class="sxs-lookup"><span data-stu-id="bcac9-131">Response</span></span>
<span data-ttu-id="bcac9-132">成功した場合、このメソッドは `202 Accepted` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="bcac9-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="bcac9-133">応答本体には何もは返されません。</span><span class="sxs-lookup"><span data-stu-id="bcac9-133">It does not return anything in the response body.</span></span> <span data-ttu-id="bcac9-134">応答には、次のヘッダーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bcac9-134">The response contains the following headers.</span></span>

| <span data-ttu-id="bcac9-135">名前</span><span class="sxs-lookup"><span data-stu-id="bcac9-135">Name</span></span>       | <span data-ttu-id="bcac9-136">説明</span><span class="sxs-lookup"><span data-stu-id="bcac9-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bcac9-137">Location</span><span class="sxs-lookup"><span data-stu-id="bcac9-137">Location</span></span>  | <span data-ttu-id="bcac9-138">要求のステータスを確認する URL です。</span><span class="sxs-lookup"><span data-stu-id="bcac9-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="bcac9-139">再試行した後</span><span class="sxs-lookup"><span data-stu-id="bcac9-139">Retry-After</span></span>  | <span data-ttu-id="bcac9-140">までの時間 (秒単位)。</span><span class="sxs-lookup"><span data-stu-id="bcac9-140">Time period in seconds.</span></span> <span data-ttu-id="bcac9-141">要求のメーカーは、これを待つ必要があります後の状態をチェックする要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="bcac9-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="bcac9-142">例</span><span class="sxs-lookup"><span data-stu-id="bcac9-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bcac9-143">要求</span><span class="sxs-lookup"><span data-stu-id="bcac9-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="bcac9-144">応答</span><span class="sxs-lookup"><span data-stu-id="bcac9-144">Response</span></span>

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
