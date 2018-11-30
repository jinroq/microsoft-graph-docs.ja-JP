---
title: 'ノートブック: getRecentNotebooks'
description: サインインしたユーザーによってアクセスされた recentNotebook インスタンスの一覧を取得します。
ms.openlocfilehash: 598d703732060f6d2074ce53c3157597c0d3cc7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021987"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="5d3dc-103">ノートブック: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="5d3dc-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="5d3dc-104">サインインしたユーザーによってアクセスされた [recentNotebook](../resources/recentnotebook.md) インスタンスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d3dc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5d3dc-105">Permissions</span></span>
<span data-ttu-id="5d3dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3dc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d3dc-108">Permission type</span></span>      | <span data-ttu-id="5d3dc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d3dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d3dc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d3dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d3dc-111">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All、</span><span class="sxs-lookup"><span data-stu-id="5d3dc-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="5d3dc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d3dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d3dc-113">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d3dc-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="5d3dc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d3dc-114">Application</span></span> | <span data-ttu-id="5d3dc-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3dc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d3dc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d3dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="5d3dc-117">ユーザーの `<id | userPrincipalName>` は、要求を行うために使用された承認トークンにおいてエンコードされたユーザーと一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-117">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="5d3dc-118">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5d3dc-118">Function parameters</span></span>

| <span data-ttu-id="5d3dc-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5d3dc-119">Parameter</span></span>    | <span data-ttu-id="5d3dc-120">型</span><span class="sxs-lookup"><span data-stu-id="5d3dc-120">Type</span></span>   |<span data-ttu-id="5d3dc-121">説明</span><span class="sxs-lookup"><span data-stu-id="5d3dc-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d3dc-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="5d3dc-122">includePersonalNotebooks</span></span>|<span data-ttu-id="5d3dc-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d3dc-123">Boolean</span></span>|<span data-ttu-id="5d3dc-124">ユーザーが所有しているノートブックを含みます。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="5d3dc-125">ユーザーが所有しているノートブックを含むには、`true` に設定します。そうでない場合は、`false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="5d3dc-126">`includePersonalNotebooks` パラメーターを含めない場合、要求は `400` エラー応答を返します。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5d3dc-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d3dc-127">Request headers</span></span>
| <span data-ttu-id="5d3dc-128">名前</span><span class="sxs-lookup"><span data-stu-id="5d3dc-128">Name</span></span>       | <span data-ttu-id="5d3dc-129">説明</span><span class="sxs-lookup"><span data-stu-id="5d3dc-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d3dc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3dc-130">Authorization</span></span>  | <span data-ttu-id="5d3dc-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5d3dc-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d3dc-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d3dc-132">Request body</span></span>
<span data-ttu-id="5d3dc-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d3dc-134">応答</span><span class="sxs-lookup"><span data-stu-id="5d3dc-134">Response</span></span>
<span data-ttu-id="5d3dc-135">正常な応答は **recentNotebooks** の JSON コレクションを含む `200 OK` を返します。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="5d3dc-136">例</span><span class="sxs-lookup"><span data-stu-id="5d3dc-136">Example</span></span>
<span data-ttu-id="5d3dc-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5d3dc-138">要求</span><span class="sxs-lookup"><span data-stu-id="5d3dc-138">Request</span></span>
<span data-ttu-id="5d3dc-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="5d3dc-140">応答</span><span class="sxs-lookup"><span data-stu-id="5d3dc-140">Response</span></span>
<span data-ttu-id="5d3dc-141">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5d3dc-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
