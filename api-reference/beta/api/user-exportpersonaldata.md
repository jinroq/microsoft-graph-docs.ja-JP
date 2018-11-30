---
title: 'ユーザー: exportPersonalData'
description: 組織のユーザーのデータをエクスポートするのには企業の管理者によって行われる、データ ポリシーの操作要求を送信します。
ms.openlocfilehash: aceab65992bde3092676a2bfa144498f07f06095
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072694"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="16d1a-103">ユーザー: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="16d1a-103">user: exportPersonalData</span></span>

<span data-ttu-id="16d1a-104">組織のユーザーのデータをエクスポートするのには企業の管理者によって行われる、データ ポリシーの操作要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="16d1a-104">Submits a data policy operation request, made by a Company Administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="16d1a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16d1a-105">Permissions</span></span>
<span data-ttu-id="16d1a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16d1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16d1a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16d1a-108">Permission type</span></span>      | <span data-ttu-id="16d1a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16d1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16d1a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16d1a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="16d1a-111">User.Export.All</span><span class="sxs-lookup"><span data-stu-id="16d1a-111">User.Export.All</span></span>  |
|<span data-ttu-id="16d1a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16d1a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="16d1a-113">該当なし</span><span class="sxs-lookup"><span data-stu-id="16d1a-113">Not applicable</span></span>  |
|<span data-ttu-id="16d1a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16d1a-114">Application</span></span> | <span data-ttu-id="16d1a-115">User.Export.All</span><span class="sxs-lookup"><span data-stu-id="16d1a-115">User.Export.All</span></span> |

><span data-ttu-id="16d1a-116">注記: エクスポートのみ実行できます企業の管理者によって委任されたアクセス許可を使用する場合。</span><span class="sxs-lookup"><span data-stu-id="16d1a-116">Note: Export can only be performed by a Company Administrator when using the delegated permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="16d1a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16d1a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="16d1a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16d1a-118">Request headers</span></span>
| <span data-ttu-id="16d1a-119">名前</span><span class="sxs-lookup"><span data-stu-id="16d1a-119">Name</span></span>       | <span data-ttu-id="16d1a-120">説明</span><span class="sxs-lookup"><span data-stu-id="16d1a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="16d1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16d1a-121">Authorization</span></span>  | <span data-ttu-id="16d1a-122">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="16d1a-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="16d1a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="16d1a-123">Request body</span></span>
<span data-ttu-id="16d1a-124">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="16d1a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="16d1a-125">パラメーター</span><span class="sxs-lookup"><span data-stu-id="16d1a-125">Parameter</span></span>    | <span data-ttu-id="16d1a-126">型</span><span class="sxs-lookup"><span data-stu-id="16d1a-126">Type</span></span>   |<span data-ttu-id="16d1a-127">説明</span><span class="sxs-lookup"><span data-stu-id="16d1a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16d1a-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="16d1a-128">storageLocation</span></span>|<span data-ttu-id="16d1a-129">String</span><span class="sxs-lookup"><span data-stu-id="16d1a-129">String</span></span>|<span data-ttu-id="16d1a-130">これは、データをエクスポートする必要があります、Azure ストレージ アカウントに共有アクセス署名 (SA) の URL です。</span><span class="sxs-lookup"><span data-stu-id="16d1a-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="16d1a-131">応答</span><span class="sxs-lookup"><span data-stu-id="16d1a-131">Response</span></span>
<span data-ttu-id="16d1a-p102">成功した場合、このメソッドは `200, OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="16d1a-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16d1a-134">例</span><span class="sxs-lookup"><span data-stu-id="16d1a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16d1a-135">要求</span><span class="sxs-lookup"><span data-stu-id="16d1a-135">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="16d1a-136">応答</span><span class="sxs-lookup"><span data-stu-id="16d1a-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
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
